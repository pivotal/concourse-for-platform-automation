# Setting the pipeline

The `pipeline.yml` use YTT.
It requires the IAASes to be tested against to be in `deployments.yml`.

```sh
fly -t ci sp -p enterprise-platform-automation -c <(ytt -f pipeline.yml -f deployments.yml )
```
