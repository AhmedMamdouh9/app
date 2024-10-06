#!/bin/bash

# Docker Login
echo $DOCKER_PASSWORD | docker login -u ahmedmamdouh51099 --password-stdin

# Docker Build
docker build -t ahmedmamdouh51099/app:latest .

# Docker Push
docker push ahmedmamdouh51099/app:latest

# Docker Logout
docker logout