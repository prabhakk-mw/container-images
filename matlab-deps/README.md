# MATLAB Dependencies

This container includes the dependencies required to run MATLAB®, Simulink®, and other MathWorks products.

**Note: This container does not include MATLAB.  To build a MATLAB container, follow [these instructions](https://github.com/mathworks-ref-arch/matlab-dockerfile).**

## Supported Tags

| Tags         | MATLAB Version | Operating System | Base Image | Usage Notes |
| ------------ |:--------------:| ---------------- |----------- | ----------- |
|[`latest`, `r2023b`, `r2023b-ubuntu22.04`, `R2023b`, `R2023b-ubuntu22.04`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2023b/ubuntu22.04/Dockerfile) | R2023b | Ubuntu 22.04 | ubuntu:22.04 | |
|[`r2023b-ubuntu20.04`, `R2023b-ubuntu20.04`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2023b/ubuntu20.04/Dockerfile) | R2023b | Ubuntu 20.04 | ubuntu:20.04 | |
|[`r2023b-ubi9`, `R2023b-ubi9`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2023b/ubi9/Dockerfile) | R2023b | Red Hat UBI 9 | registry.access.redhat.​com/ubi9/ubi:latest | |
|[`r2023b-ubi8`, `R2023b-ubi8`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2023b/ubi8/Dockerfile) | R2023b | Red Hat UBI 8 | registry.access.redhat.​com/ubi8/ubi:latest | |
|[`r2023b-aws-batch`, `R2023b-aws-batch`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2023b/aws-batch/Dockerfile) | R2023b | Ubuntu 22.04 | nvidia/cuda:11.8.0-base-ubuntu22.04 | For use with [MATLAB® Parallel Server™ with AWS® Batch](https://github.com/mathworks-ref-arch/matlab-parallel-server-with-aws-batch)|
|[`r2023a`, `r2023a-ubuntu20.04`, `R2023a`, `R2023a-ubuntu20.04`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2023a/ubuntu20.04/Dockerfile) | R2023a | ubuntu:20.04 | ubuntu:20.04 | |
|[`r2023a-ubuntu22.04`, `R2023a-ubuntu22.04`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2023a/ubuntu22.04/Dockerfile) | R2023a | Ubuntu 22.04 | ubuntu:22.04 | |
|[`r2023a-ubi8`, `R2023a-ubi8`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2023a/ubi8/Dockerfile) | R2023a | Red Hat UBI 8 | registry.access.redhat.​com/ubi8/ubi:latest | |
|[`r2023a-ubi9`, `R2023a-ubi9`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2023a/ubi8/Dockerfile) | R2023a | Red Hat UBI 9 | registry.access.redhat.​com/ubi9/ubi:latest | |
|[`r2023a-aws-batch`, `R2023a-aws-batch`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2023a/aws-batch/Dockerfile) | R2023a | Ubuntu 20.04 | nvidia/cuda:11.8.0-base-ubuntu20.04 | For use with [MATLAB® Parallel Server™ with AWS® Batch](https://github.com/mathworks-ref-arch/matlab-parallel-server-with-aws-batch)|
|[`r2022b`, `r2022b-ubuntu20.04`, `R2022b`, `R2022b-ubuntu20.04`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2022b/ubuntu20.04/Dockerfile) | R2022b | Ubuntu 20.04 | ubuntu:20.04 | |
|[`r2022b-ubuntu22.04`, `R2022b-ubuntu22.04`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2022b/ubuntu22.04/Dockerfile) | R2022b | Ubuntu 22.04 | ubuntu:22.04 | |
|[`r2022b-ubi8`, `R2022b-ubi8`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2022b/ubi8/Dockerfile) | R2022b | Red Hat UBI 8 | registry.access.redhat.​com/ubi8/ubi:latest | |
|[`r2022b-ubi9`, `R2022b-ubi9`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2022b/ubi9/Dockerfile) | R2022b | Red Hat UBI 9 | registry.access.redhat.​com/ubi9/ubi:latest | |
|[`r2022b-aws-batch`, `R2022b-aws-batch`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2022b/aws-batch/Dockerfile) | R2022b | Ubuntu 20.04 | nvidia/cuda:11.8.0-base-ubuntu20.04 | For use with [MATLAB® Parallel Server™ with AWS® Batch](https://github.com/mathworks-ref-arch/matlab-parallel-server-with-aws-batch)|
|[`r2022a`, `r2022a-ubuntu20.04`, `R2022a`, `R2022a-ubuntu20.04`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2022a/ubuntu20.04/Dockerfile) | R2022a | Ubuntu 20.04 | ubuntu:20.04 | |
|[`r2022a-ubi8`, `R2022a-ubi8`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2022a/ubi8/Dockerfile) | R2022a | Red Hat UBI 8 | registry.access.redhat.​com/ubi8/ubi:latest | |
|[`r2022a-aws-batch`, `R2022a-aws-batch`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2022a/aws-batch/Dockerfile) | R2022a | Ubuntu 20.04 | nvidia/cuda:11.8.0-base-ubuntu20.04 | For use with [MATLAB® Parallel Server™ with AWS® Batch](https://github.com/mathworks-ref-arch/matlab-parallel-server-with-aws-batch)|
|[`r2021b`, `r2021b-ubuntu20.04`, `R2021b`, `R2021b-ubuntu20.04`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2021b/ubuntu20.04/Dockerfile) | R2021b | Ubuntu 20.04 | ubuntu:20.04 | |
|[`r2021b-ubi8`, `R2021b-ubi8`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2021b/ubi8/Dockerfile) | R2021b | Red Hat UBI 8 | registry.access.redhat.​com/ubi8/ubi:latest | |
|[`r2021b-aws-batch`, `R2021b-aws-batch`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2021b/aws-batch/Dockerfile) | R2021b | Ubuntu 20.04 | nvidia/cuda:11.8.0-base-ubuntu20.04 | For use with [MATLAB® Parallel Server™ with AWS® Batch](https://github.com/mathworks-ref-arch/matlab-parallel-server-with-aws-batch)|
|[`r2021a`, `r2021a-ubuntu20.04`, `R2021a`, `R2021a-ubuntu20.04`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2021a/ubuntu20.04/Dockerfile) | R2021a | Ubuntu 20.04 | ubuntu:20.04 | |
|[`r2021a-aws-batch`, `R2021a-aws-batch`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2021a/aws-batch/Dockerfile) | R2021a | Ubuntu 20.04 | nvidia/cuda:11.8.0-base-ubuntu20.04 | For use with [MATLAB® Parallel Server™ with AWS® Batch](https://github.com/mathworks-ref-arch/matlab-parallel-server-with-aws-batch)|
|[`r2020b`, `r2020b-ubuntu20.04`, `R2020b`, `R2020b-ubuntu20.04`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2020b/ubuntu20.04/Dockerfile) | R2020b | Ubuntu 20.04 | ubuntu:20.04 | |
|[`r2020b-aws-batch`, `R2020b-aws-batch`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2020b/aws-batch/Dockerfile) | R2020b | Ubuntu 20.04 | nvidia/cuda:11.8.0-base-ubuntu20.04 | For use with [MATLAB® Parallel Server™ with AWS® Batch](https://github.com/mathworks-ref-arch/matlab-parallel-server-with-aws-batch)|
|[`r2020a`, `r2020a-ubuntu18.04`, `R2020a`, `R2020a-ubuntu18.04`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2020a/ubuntu18.04/Dockerfile) | R2020a | Ubuntu 18.04 | ubuntu:18.04 | |
|[`r2020a-aws-batch`, `R2020a-aws-batch`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2020a/aws-batch/Dockerfile) | R2020a | Ubuntu 18.04 | nvidia/11.8.0-base-ubuntu18.04 | For use with [MATLAB® Parallel Server™ with AWS® Batch](https://github.com/mathworks-ref-arch/matlab-parallel-server-with-aws-batch)|
|[`r2019b`, `r2019b-ubuntu18.04`, `R2019b`, `R2019b-ubuntu18.04`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2019b/ubuntu18.04/Dockerfile) | R2019b | Ubuntu 18.04 | ubuntu:18.04 | |
|[`r2019b-aws-batch`, `R2019b-aws-batch`](https://github.com/mathworks-ref-arch/container-images/blob/main/matlab-deps/r2019b/aws-batch/Dockerfile) | R2019b | Ubuntu 18.04 | nvidia/cuda:11.8.0-base-ubuntu18.04 | For use with [MATLAB® Parallel Server™ with AWS® Batch](https://github.com/mathworks-ref-arch/matlab-parallel-server-with-aws-batch)|

## License
The license for this container is available [here](https://github.com/mathworks-ref-arch/container-images/blob/main/LICENSE.md).

## Security Reporting
To report suspected security issues, follow [these instructions](https://github.com/mathworks-ref-arch/container-images/blob/main/SECURITY.md).

## Technical Support
If you require assistance or have a request for additional features or capabilities, please contact [MathWorks Technical Support](https://www.mathworks.com/support/contact_us.html).

----

Copyright 2019-2023 The MathWorks, Inc.

----