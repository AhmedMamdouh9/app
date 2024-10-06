#!/bin/bash

# Docker Login
echo $DOCKER_PASSWORD | docker login -u ahmedmamdouh51099 --password-stdin

# Docker Build
docker build -t ahmedmamdouh51099/app:latest .

# Docker Push
docker push ahmedmamdouh51099/app:latest

# Test
echo "Test message: Docker image has been built and pushed successfully."