# webpage

* https://github.com/halogenica/beautifulhugo
* https://gohugo.io/getting-started/quick-start/
* Example: https://hugo-theme-beautifulhugo.netlify.app/

## Hugo installation

Get a recent version, such as

```sh
$ hugo version
hugo v0.152.2-6abdacad3f3fe944ea42177844469139e81feda6+extended linux/amd64 BuildDate=2025-10-24T15:31:49Z VendorInfo=snap:0.152.2
```

## Mac installation

As the theme is installed as a go module you may run into an error message if there's no go available:

```
Error: command error: failed to load modules: failed to download modules: failed to execute 'go [mod download]': failed to execute binary "go" with args [mod download]: go: go.mod requires go >= 1.25.5 (running go 1.25.3)
 *errors.errorString
```

```sh
$ brew install go
```

## Linux installation

```sh
$ sudo snap install go --classic
go 1.25.5 from Canonical✓ installed
```

## Local development

```sh
cd site
hugo serve
```
