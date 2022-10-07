# CapStoneGBD


Deploying Flask HelloWorld application in AWS EKS

#Environment

Application     - Flask Hello World
CI Tool         - CircleCI
Deployment Type - Rolling Deployment


#Files
.circleci/config.yml          - circleci config file
flaskapp/app.py               - application file
Dockerfile                    - Docker script to build image
Makefile                      - Project make file
ekscluster.yml                - cloud formation script for eks cluster
deployment.yml                - deploy script
requirements.txt              - python pip requirements list
