# Offsiteworking.com
Static website for Offsetworking.com hosted on s3 bucket. 

## Git setup
Local VS code has two branches dev & deploy. The dev branch is for local development. 

Once the dev branch is ready to deploy use `git push origin dev:deploy` in the local terminal to push the local dev branch to the github.com deploy branch. 

The deploy branch is configured with a CodePipeline in the `106687886560` AWS account to push the code from github.com to the s3 bucket which is hosting the static site. 

## Domain
The domain was housed in the `host-simplew7` enom account. 

The DNS is pointed to Route53 `106687886560` AWS account. Route53 is pointed to the s3 bucket in the same AWS account configured to serve static files. 