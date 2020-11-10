# gitpod



[![Open in Gitpod](https://camo.githubusercontent.com/1eb1ddfea6092593649f0117f7262ffa8fbd3017/68747470733a2f2f676974706f642e696f2f627574746f6e2f6f70656e2d696e2d676974706f642e737667)](https://gitpod.io/#https://github.com/co2zxc/gitpod)


## Create AWS CDK App

```bash
npx projen new awscdk-app-ts
```




## Request temporary credentials and update ~/.aws/credentials

```sh
$ bash utils/refresh_credentials.sh 
=> requesting temporary credentials
=> updating ~/.aws/credentials as profile default
[OK] done
```
If you have different SSO profile name, run it with `AWS_PROFILE`:

```sh
$ AWS_PROFILE=<OTHER_PROFILE_NAME> bash utils/refresh_credentials.sh 
```

## Start your CDK development

You should be able to run the CDK CLI now.

```sh
$ cdk diff
$ cdk deploy
$ cdk destroy
```
