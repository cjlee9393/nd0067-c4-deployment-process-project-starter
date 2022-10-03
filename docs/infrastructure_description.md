# Infrasctructure Description
Document the infrastructure needs (RDS, S3 Elastic Beanstalk, etc) AWS services used for hosting the API, Frontend, and the DB.

## RDS
1. Class: db.t3.micro
1. Engine: PostgreSQL
1. Role: Instance
1. Endpoint: database-1.cerp5xfjafrr.us-east-1.rds.amazonaws.com
1. Port: 5432

## S3
1. Role: Instance
1. Endpoint: http://myawsbucket-2028006.s3-website-us-west-1.amazonaws.com/

## Elastic Beanstalk
1. Platform: Node.js 14 running on 64bit Amazon Linux 2/5.5.6
1. Role: Instance
1. Endpoint: udagram-api-dev.us-west-1.elasticbeanstalk.com