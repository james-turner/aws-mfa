# Prerequisites

You should already have run `aws configure` and have an access key and secret under ~/.aws/credentials

# Installation

    \curl -sSL https://raw.githubusercontent.com/james-turner/aws-mfa/master/installer | bash


Now you can run the normal aws commands and you'll get prompted for MFA if your current token has expired.
