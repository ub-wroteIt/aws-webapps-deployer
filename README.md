# aws-webapps-deployer
This repository contains cloudformation script which deploys webapps into AWS ecosystem. 

## Prerequisites

You must have AWS account, Secrete key, Access Keys of the account and AWS-CLI tool.

## Usage

Upload your codebase as zip file into s3 bucket. Make sure that bucket is accessible thorough the role you create. Name that role as S3_Full_ACCESS.

execute the bash scripts provided in the Helper directory.

```
../Helper/create.sh networkinfra ../cloudformation-scripts/Networking-Resources/networking-resources.yml ../cloudformation-scripts/Networking-Resources/networking-resources-parameters.json

../Helper/create.sh serverinfra ../cloudformation-scripts/Computing-Resources/compute-resources.yml ../cloudformation-scripts/Computing-Resources/compute-resources-parameters.json

```

