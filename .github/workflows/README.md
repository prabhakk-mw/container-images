# Build, Test, and Publish the Dockerfile

> This folder is intended only for the administrators of the container-images repository. 

The workflow in this folder builds and publishes a Docker images to DockerHub.

## Triggers and Scheduled Jobs

The workflow is scheduled to run every Monday at 00:00.

Additionally, the workflow is triggered each time you push a change in the [`Dockerfile`](../../Dockerfile).

You can also trigger the workflow from the "Actions" tab.

## Directory structure

The container-images repository contains the following directory structure:

The root directory of the repository lists the various container images that this repository hosts.
There after called `BASE_IMAGE`.

1. matlab-deps
2. polyspace-deps
3. matlab-runtime-deps (From R2023b)

Each of these directories lists various releases of MATLAB:
Here after called `MATLAB_RELEASE`.

1. r2019b
2. r2020a ... and so on

Each of these directories may have one or more OS Flavors listed:
Here after called `OS`
1. aws-batch
2. ubi8 / ubi9
3. ubuntu20.04 / ubuntu22.04

Each of these directories should have a `Dockerfile` and some accompanying files:

1. Dockerfile
2. base-dependencies.txt
3. *.sh `(scripts)`

## Image pushed to DockerHub:
Two tags are created: 
1. The letter `r` in lower case in `MATLAB_RELEASE`. Here after called: `r_MATLAB_RELEASE`
2. The letter `R` is upper case in `MATLAB_RELEASE`. Here after called: `R_MATLAB_RELEASE`

The images pushed per Dockerfile will use the following naming schema:
` mathworks/${BASE_IMAGE}:${r_MATLAB_RELEASE}-${OS} `
` mathworks/${BASE_IMAGE}:${R_MATLAB_RELEASE}-${OS} `

### Latest Tag
Every `BASE_IMAGE` would need to tag which `MATLAB_RELEASE` & `OS` flavor marks its `latest` image.

## Workflow Description

The workflow consists of a one-dimensional matrix of jobs. Each job builds, tests and publishes the container image for a different MATLAB release, starting from `r2020b`. To ensure that a failure in any job does not cancel other jobs, the `fail-fast` option is set to `false`.

Each job consists of the following steps:

1. Check-out the repository into a GitHub Actions runner.
2. Login to ghcr.io, the GitHub Container Registry.
3. Build the image locally (set the `load` variable to `true`, as suggested in [this example](https://github.com/docker/build-push-action/blob/master/docs/advanced/test-before-push.md)).
4. Install Python and the PyPi packages listed in [`requirements.txt`](../../tests/requirements.txt).
5. Run the tests.
6. Rebuild and push the image to the GitHub Container Registry if the image passed all the tests.
