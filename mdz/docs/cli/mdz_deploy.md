## mdz deploy

Deploy a new deployment

### Synopsis

Deploys a new deployment directly via flags.

```
mdz deploy [flags]
```

### Examples

```
  mdz deploy --image=modelzai/llm-blomdz-560m:23.06.13
  mdz deploy --image=modelzai/llm-blomdz-560m:23.06.13 --name blomdz-560m --node-labels gpu=true,name=node-name
```

### Options

```
  -h, --help                  help for deploy
      --image string          Image to deploy
      --max-replicas int32    Maximum number of replicas (default 1)
      --min-replicas int32    Minimum number of replicas (can be 0) (default 1)
      --name string           Name of inference
  -l, --node-labels strings   Node labels
      --port int32            Port to deploy on (default 8080)
```

### Options inherited from parent commands

```
      --debug        Enable debug logging
  -u, --url string   URL to use for the server (MDZ_URL) (default http://localhost:80)
```

### SEE ALSO

* [mdz](mdz.md)	 - mdz manages your deployments

###### Auto generated by spf13/cobra on 26-Jul-2023
