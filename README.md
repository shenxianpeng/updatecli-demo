# updatecli-demo

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/shenxianpeng/updatecli-demo)


## Install

https://www.updatecli.io/docs/prologue/installation/

I'm using Ubuntu

```bash
curl -sL -o/var/cache/apt/archives/updatecli_amd64.deb https://github.com/updatecli/updatecli/releases/download/v0.71.0/updatecli_amd64.deb
sudo apt install /var/cache/apt/archives/updatecli_amd64.deb
```

## Quick Start

```bash
# To see what would change
updatecli diff --config manifest.yaml

# To apply the change
updatecli apply --config manifest.yaml

# Then data.yaml will be updated
$ git diff data.yaml
diff --git a/data.yaml b/data.yaml
index a577b14..fd848ef 100644
--- a/data.yaml
+++ b/data.yaml
@@ -1,3 +1,3 @@
 container:
   image: jenkinsci/jenkins
-  tag: 2.275
+  tag: "2.403"
```