# aws-lambda-rekog-sns-s3-python 🐳

![Stars](https://img.shields.io/github/stars/tquangdo/aws-lambda-rekog-sns-s3-python?color=f05340)
![Issues](https://img.shields.io/github/issues/tquangdo/aws-lambda-rekog-sns-s3-python?color=f05340)
![Forks](https://img.shields.io/github/forks/tquangdo/aws-lambda-rekog-sns-s3-python?color=f05340)
[![Report an issue](https://img.shields.io/badge/Support-Issues-green)](https://github.com/tquangdo/aws-lambda-rekog-sns-s3-python/issues/new)

![overview](screenshots/overview.png)

## reference
[youtube](https://www.youtube.com/watch?v=wnTvVB1ojPk&t=3s)

## IAM role
- role name=`DTQRoleRekog`
![role](screenshots/role.png)

## SNS
- topic name=`DTQSNSTopicRekog`
- subscription: email=`xxx@gmail.com` > confirm by email

## S3
- bucket name=`dtq-bucket-rekog`

## lambda
1. options=`blue print` > KW=`rekog`> choose `rekognition-python`
2. name=`DTQLambdaRekog`
3. role=`DTQRoleRekog`
4. bucket=`dtq-bucket-rekog`
5. Suffix=`.jpeg`
6. code: delete blue print default code: delete function has KW=`face` > add code for "sns"
![lambda](screenshots/lambda.png)
- upload `images/fruits.jpeg` into `dtq-bucket-rekog`
![res](screenshots/res.png)
