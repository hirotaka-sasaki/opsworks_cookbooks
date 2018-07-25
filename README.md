# opsworks_cookbooks
This is cookbooks for Rails Application.

## DelayedJob Configuration
### Custom JSON of Opsworks
```
}
  "delayed_job": {
    "pool_size": 1, "path_to_script": "bin"
  }
}
```
## PaperTrail
### Custom JSON of Opsworks
```
{
  "papertrail": {
    "remote_host": "logs2.papertrailapp.com",
    "remote_port": "[PORT]",
    "watch_files": {
      "/srv/www/[APP_NAME]/shared/log/production.log" : "rails" ,
      "/srv/www/[APP_NAME]/shared/log/batch.log" : "batch"
    }
  }
}
```
## Redis
Please read README of below github link.
https://github.com/hirotaka-sasaki/redis_opsworks_cookbook
