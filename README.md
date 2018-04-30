# Heptio Ark

Heptio Ark enables the ability to take backups of EBS volumes on a configurable
schedule. These backups can be given a TTL to help save costs.

# Release History

## 1.0.0 (April 29 2018)

* Initial release.

#To set up Ark on AWS, :

*  Create  S3 bucket,
*  Create an AWS IAM role for Ark,
*  Configure the server,
*  Add kube2iam annotation in deployment.
