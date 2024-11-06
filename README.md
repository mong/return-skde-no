## Administer return-skde-no
Easy way of working with AWS EB: [install eb cli](https://github.com/aws/aws-elastic-beanstalk-cli-setup)

### Make EB environment (first time use)
In bash:
```bash
eb init return-skde-no
eb create -r eu-west-1 -i t1.micro --elb-type application return-skde-no
```

### Deploy (every update)
In bash:
```bash
export AWS_ACCESS_KEY_ID=<id>
export AWS_SECRET_ACCESS_KEY=<token>
export AWS_DEFAULT_REGION=eu-west-1

eb deploy return-skde-no
```
