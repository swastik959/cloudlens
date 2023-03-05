<p align="center">
      <img src="assets/cloudlens.png" alt="Cloudlens" width="225" height="150" >
</p>

## Cloudlens - k9s like CLI for AWS. 

![](./assets/cloudlensdemo.gif)

Cloudlens provides a terminal UI for AWS Service Management and Monitoring! With its easy to use UI and advanced features, you can easily navigate, observe, and optimize your AWS environment. Whether you're a cloud expert or just getting started, cloudlens will elevate your AWS experience and take your service management to new heights.

## Installation

Cloudlens is available on Linux and macOS.

* Via [Homebrew](https://brew.sh/) for macOS or Linux

   ```shell
   brew install one2nc/cloudlens/cloudlens
   ```

* Building from source code
      Cloudlens is currently in active development. We use Go 1.19. Follow these steps to build cloudlens locally:

       1. Clone the repo
       2. Build and run the executable

  To Run:
  ```shell
  make run
  ```

## Usage

For the simple usage, just run the command without any options.

```shell
cloudlens
```

For knowing all the options available, use:
```shell
cloudlens help
```

## Features

Our terminal application supports various features, allowing users to view EC2 instances, S3 buckets, EBS volumes, VPCs, SQS queues, Lambda functions, subnets, security groups, and IAM roles, making their work faster and more efficient.

## Screenshots

1. EC2
      <img src="assets/ec2.png"/>
1. EC2 Details
      <img src="assets/ec2Details.png"/>

2. S3
      <img src="assets/S3.png"/>
2. S3 Details
      <img src="assets/S3Details.png"/>

## Documentation

Please refer to our [Cloudlens documentation](https://one2n.gitbook.io/docs/) to know more.


## Key Bindings

Cloudlens uses k9s like shortcuts for navigation. Listed below are few of the shortcuts:

| **Action**                                | **Command**   |
|-------------------------------------------|---------------|
| Show active keyboard mnemonics and help   | ?             |
| To bail out of cloudlens                  | :q ,   ctrl-c |
| Bails out of view/command/filter mode     | esc         |
| To view and switch to another AWS Service | :S3/EC2/VPC⏎  |

## Note
**Cloudlens reads your ~/.aws/config file, but it does not store or send your access and secret key anywhere. The access and secret key is used only to securely connect to AWS API via AWS SDK.**

**Since cloudlens is in readonly mode, we recommend you create an access and secret key that only has readonly permissions to the AWS services.**

## Acknowledgements

We would like to express our sincere appreciation to `K9s` as it has been a invaluable source of reference for this project.

All materials licensed under [Apache v2.0](http://www.apache.org/licenses/LICENSE-2.0)

## We appreciate [localstack's](https://localstack.cloud/) assistance with the development

<img src="assets/localstack.jpeg" alt="k9s">
