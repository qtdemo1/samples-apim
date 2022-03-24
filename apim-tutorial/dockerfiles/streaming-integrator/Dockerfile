# use streaming-integrator-base-image
FROM docker.io/wso2/wso2si:4.0.0
MAINTAINER WSO2 Docker Maintainers "dev@wso2.org"

ARG HOST_APPS_DIR=./siddhi-files
ARG SAMPLES_DIR=${WSO2_SERVER_HOME}/samples/artifacts/
ARG APPS=${WSO2_SERVER_HOME}/deployment/siddhi-files
ARG CONFIG_FILE=./configurations.yaml
ARG CONFIG_FILE_PATH=${HOME}/configurations.yaml

# copy bundles & jars to the siddhi-runner distribution
COPY ${HOST_APPS_DIR}/ ${APPS}

# # copy deployment.yaml with service catalog configs
# COPY deployment.yaml ${WSO2_SERVER_HOME}/conf/server/
