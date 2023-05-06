

```bash
docker run -v "$PWD/manifest.yaml":/updatecli/manifest.yaml:ro ghcr.io/updatecli/updatecli:latest diff --config /updatecli/manifest.yaml
```