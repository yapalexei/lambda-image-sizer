# Lambda imageSizer

Based on the AWS example docs, this function is a spin off of an image converter.

## Basic Functionality

All this does is that it listens for S3 bucket `ObjectCreated` events and starts a conversion process of an image.
It then takes the converted image tumb and places it in the "Thumbs Bucket" for use.

## Setup

Be sure to run `npm install` as this will download and install the deps for this function. After this, change the "dstBucket" value
in the code to match the name of your bucket if you want this to work for you. Then, zip "imageSizer.js" and the "node_modules" folder to then upload and use on AWS Lambda.