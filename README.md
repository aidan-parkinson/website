# Website for Aidan Thmomas Parkinson

This website has been created from a bootstrap application. Designed for hosting on a web server.

## To deploy on Amazon Web Services

1. Create a private AWS S3 bucket and upload all content within repository.

2. Create an AWS Cloudfront distribution for the AWS S3 bucket created and set origin to `home.html`.

3. Make the AWS S3 bucket public by taking the steps to apply a security policy shown here:
`https://aws.amazon.com/premiumsupport/knowledge-center/cloudfront-access-to-amazon-s3/`

4. Add a CNAME record for the AWS Cloudfront distribution created for access `https://aidanparkinson.xyz`

5. Use AWS Certificate Manager to generate an SSL certificate for the CNAME record and apply to AWS Cloudfront distribution created.
