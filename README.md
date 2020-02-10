# Docker Image with Homebrew and AWS CLI 

Alpine with AWS CLI and Homebrew

## Build

```
docker build -t milldr/amazon-brew .
```

Automated build on Docker Hub

[![DockerHub Badge](http://dockeri.co/image/milldr/amazon-brew)](https://hub.docker.com/r/milldr/amazon-brew/)

## Usage

Configure:

```
export AWS_ACCESS_KEY_ID="<id>"
export AWS_SECRET_ACCESS_KEY="<key>"
export AWS_DEFAULT_REGION="<region>"
```

## Maintenance

- The Docker image build & publish is automated by CircleCI 
- The awscli and s3cmd packages have handcoded versions in the Dockerfile that need to be bumped manually.

## References

- AWS CLI Docs: https://aws.amazon.com/documentation/cli/
- Homebrew: https://docs.brew.sh/Homebrew-on-Linux

