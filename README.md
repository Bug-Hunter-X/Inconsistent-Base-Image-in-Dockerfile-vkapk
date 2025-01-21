# Inconsistent Base Image in Dockerfile

This repository demonstrates a common mistake in Dockerfiles: using `ubuntu:latest` as the base image.  This can lead to inconsistencies between builds due to updates in the base image.  The solution shows how to specify a specific version for reproducibility and stability. 

## Bug
The original Dockerfile uses `ubuntu:latest`.  This is problematic because the contents of `ubuntu:latest` can change, leading to different build results over time. 

## Solution
The fixed Dockerfile specifies a particular version of Ubuntu (e.g., `ubuntu:22.04`).  This ensures that the build process always uses the same base image, improving reproducibility and reducing the risk of unexpected changes.