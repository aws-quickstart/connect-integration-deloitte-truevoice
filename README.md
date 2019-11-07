# quickstart-deloitte-truevoice

## TrueVoice Registration and Integration

Deploying this Quick Start provides registration and proposed onboarding information for validation by the TrueVoice customer engagement team. After successful registration and due-diligence procedures are completed by TrueVoice, an AWS Service Catalog Product will be made available to users, which provides a multipurpose TrueVoice PoV integration layer for use with AWS Connect, Corporate Data Center, or AWS Management Console uploads to Amazon S3:

![Quick Start architecture for TrueVoice Registration and Integration](https://d0.awsstatic.com/partner-network/QuickStart/connect/connect-integration-deloitte-truevoice-architecture.png)

This Quick Start sets up the following:

•	A registration stack consisting of a Custom Resource Lambda function that will invoke the TrueVoice PoV registration API and return a registration ID as a CloudFormation output.

After successful registration, an AWS Service Catalog Product will be made available to the account from where the Quick Start was launched, providing a template that sets up the following:

•	An S3 bucket intended for integration with customer-dedicated resources in the TrueVoice AWS account and used as a staging area for audio files sourced from on-premises telephony systems or Amazon Connect.

•	A Lambda function tasked with transferring files from the customer’s integration bucket to the TrueVoice AWS account.

•	The required Lambda AWS Identity and Access Management (IAM) Execution Role to carry out the transfer from the integration bucket to the customer-dedicated resources in the TrueVoice AWS account.

For architectural details, best practices, step-by-step instructions, and customization options, see the [deployment guide](https://fwd.aws/7yBxp).

To post feedback, submit feature ideas, or report bugs, use the Issues section of this GitHub repo.

If you'd like to submit code for this Quick Start, please review the [AWS Quick Start Contributor's Guide](https://aws-quickstart.github.io/).
