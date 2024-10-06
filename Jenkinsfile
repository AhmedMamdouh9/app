#!/bin/bash

# Docker Login
echo $DOCKER_PASSWORD | docker login -u ahmedmamdouh51099 --password-stdin
if [ $? -ne 0 ]; then
    echo "Docker login failed"
    exit 1
fi

# Docker Build
docker build -t ahmedmamdouh51099/app:latest .
if [ $? -ne 0 ]; then
    echo "Docker build failed"
    exit 1
fi

# Docker Push
docker push ahmedmamdouh51099/app:latest
if [ $? -ne 0 ]; then
    echo "Docker push failed"
    exit 1
fi

# Test
echo "Test message: Docker image has been built and pushed successfully."