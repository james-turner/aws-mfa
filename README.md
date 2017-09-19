# Prerequisites

You should already have run `aws configure` and have an access key and secret under ~/.aws/credentials

You require python installed (any version should be fine - submit a PR fix if not).

# Installation

    \curl -sSL https://raw.githubusercontent.com/james-turner/aws-mfa/master/installer | bash


Now you can run the normal aws commands and you'll get prompted for MFA if your current token has expired.

Expected output should look something like this:


    $> aws ec2 describe-instances
    Using device: arn:aws:iam::ACCOUNT_NUMER:mfa/USERNAME
    Enter your mfa code:
    XXXXXX
    Credentials updated
    ...
