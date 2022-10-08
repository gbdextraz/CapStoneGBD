# CapStoneGBD

Deploying Flask HelloWorld application in AWS EKS

# Project GitHub Repo

    https://github.com/gbdextraz/CapStoneGBD/

# Environment

- Application     - Flask Hello World
- CI Tool         - CircleCI
- Deployment Type - Rolling Deployment


# Files
- .circleci/config.yml          - circleci config file
- flaskapp/app.py               - application file
- Dockerfile                    - Docker script to build image
- Makefile                      - Project make file
- ekscluster.yml                - cloud formation script for eks cluster
- deployment.yml                - deploy script
- requirements.txt              - python pip requirements list

# Steps

##  Test Docker Build Locally

```
docker build --tag=capstone .
docker image list
docker run -p 8000:80 capstone
```

## Create EKS
```
eksctl create cluster -f ekscluster.yml --dry-run
eksctl create cluster -f ekscluster.yml
```
