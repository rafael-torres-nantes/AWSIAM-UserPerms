# AWSIAM-UserPerms

Cria o user no root
Cria no Security Credentials uma Acess Key
Faça a configuraçã
```bash
aws configure
```

Com o user configurado, faça isso:
```bash
aws sts get-caller-identity
```
```
{
    "UserId": "XXXXXXXXXXXXX",
    "Account": "XXXXXXXXXXXX",
    "Arn": "arn:aws:iam::147997118975:user/RafaTorresminho"
}
```

```bash
aws sts get-session-token --duration-seconds 7200
```

```
{
    "Credentials": {
        "AccessKeyId": "XXXXXXXXXXXXX",
        "SecretAccessKey": "YYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYY",
        "SessionToken": "ZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZ",
        "Expiration": "2025-01-21T17:30:15+00:00"
    }
}
```
