
## For local development

Fill in a secret value in the `.env` file.

For local development, use this random string as an appropriate value:

```shell
SECRET_KEY=123abc
```

## When you deploy to Azure Web apps Linux

For deployment to production, create an app setting, `SECRET_KEY`. Use this command to generate an appropriate value:

```shell
python -c 'import secrets; print(secrets.token_hex())'
```

Trigger new build
