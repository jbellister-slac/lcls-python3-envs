# LCLS Python Environments

A repository for holding yaml files representing conda environments for use on the SLAC network. Also includes workflows for creating and testing the environments for deployment to RHEL6 and RHEL7 machines. The environments described by the files are as follows:

## default-rhel7-environment

This is the environment that will be available to anyone logging into a RHEL7 box and sourcing the default startup scripts. Intended to be stable, only updated via CATER requests, suitable for running production applications.

## default-rhel6-environment

This is the old default environment, only for use on any remaining machines still running RHEL6.

## nightly-rhel7-environment

Updated via [cron job](https://github.com/slaclab/lcls-python3.8-env/blob/main/.github/workflows/publish_rhel7_nightly.yml) to obtain more recent versions of packages.

## Documentation

For additional documentation including the GitHub actions that support the build and testing process please see here: https://slaclab.github.io/conda-pack-docs/
