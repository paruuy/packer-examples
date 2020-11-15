# PACKER Examples

This examples are executing in AWS, for these reason you will need an aws account.

To execute this examples you will need to install in your machine packer: <https://learn.hashicorp.com/tutorials/packer/getting-started-install>

If you prefer using packer in a docker image: docker run -it -v $PWD:/app -w /app --entrypoint "" hashicorp/packer:light sh
After that, you need to create the environment variables for AWS credentials:

export AWS_ACCESS_KEY_ID=<YOUR_AWS_IAM_KEY_ID>
export AWS_SECRET_ACCESS_KEY=<YOUR_AWS_IAM_SECRET_KEY>

More information: <https://www.packer.io/docs/builders/amazon#environment-variables>

## Provisioners Example

If you are using the docker image of packer, to use ansible provisioner will be necessary install ansible in the docker image, for these reason you need to execute: apk -U add ansible
