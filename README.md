# minio-azure-deisapp
minio azure gateway running on Deis cmd.

## How To

You must get your storage account for Azure Blob.
app-name is as you like.

```
deis create {{app-name}} --no-remote
deis config:set -a {{app_name}} MINIO_ACCESS_KEY={{azureaccountname}} MINIO_SECRET_KEY={{azureaccountkey}}
deis pull -a {{app_name}} monami0ya/minio-azure-deisapp
```

You can access via http://{{app-name}}.{{your-deis-domain}}/ after deployment.
