# Pre-built Dev Container Image for R. More info: https://github.com/rocker-org/devcontainer-images/pkgs/container/devcontainer%2Ftidyverse
# Available R version: 4, 4.1, 4.2, 4.3
ARG VARIANT="4"
FROM ghcr.io/rocker-org/devcontainer/tidyverse:${VARIANT}

RUN install2.r --error --skipinstalled -n -1 \
        kableExtra \
        flextable \
        RcppAlgos \
    && rm -rf /tmp/downloaded_packages
