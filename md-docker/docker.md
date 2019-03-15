[&#8592; Index](../README.md)
## Cleanup commands
- Remove all stopped containers:

```bash
docker rm $(docker ps -a -q)
```

- Remove all dangling (i.e. untagged) images:

```bash
docker rmi $(docker images --quiet --filter "dangling=true")
```
