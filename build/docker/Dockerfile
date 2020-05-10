ARG STEP_1_IMAGE=golang:1.14.1-alpine3.11
FROM ${STEP_1_IMAGE} AS STEP_1

ARG GITHUB_HEAD_REF="master"
ARG GITHUB_EVENT_NAME="push"

# Add github
RUN apk update && \
    apk upgrade && \
    apk add --no-cache \
        git \
        make \
        bash

