# Cygni Tech Summit 2017 AWS demo

## Pre-setup

1. Log in to AWS console, on the eu-central-1 region
1. Setup empty S3 bucket. Note the name.

## Installation / Launch

1. Create lambda function named "watermarker"
1. Set timeout 10 seconds, max memory 256 MB.
1. Run ./create-lambda-package.sh from project directory to create the deploy.zip file
1. Upload zip file
1. Tie trigger from S3 bucket created above for "ObjectCreated" events
1. Enable event trigger
