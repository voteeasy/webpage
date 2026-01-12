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

## How to get theme updates?

In case you installed as hugo module:

```sh
$ hugo mod get
```

Download starts and you will get the following diff:

```sh
diff --git a/site/go.mod b/site/go.mod
index c21a339..6a0bc4e 100644
--- a/site/go.mod
+++ b/site/go.mod
@@ -2,4 +2,4 @@ module github.com/voteeasy/webpage

go 1.25.3

-require github.com/halogenica/beautifulhugo v0.0.0-20251212183709-c3c3bbb7370d // indirect
+require github.com/halogenica/beautifulhugo v0.0.0-20260112152821-6173aa260601 // indirect
diff --git a/site/go.sum b/site/go.sum
index 5fe239b..cf39796 100644
--- a/site/go.sum
+++ b/site/go.sum
@@ -1,2 +1,4 @@
github.com/halogenica/beautifulhugo v0.0.0-20251212183709-c3c3bbb7370d h1:EsekjF0bASegdBSWPTnc8l0fhsmv/w7jmO2XgEpCItU=
github.com/halogenica/beautifulhugo v0.0.0-20251212183709-c3c3bbb7370d/go.mod h1:4dwHt6njigk+fr9W3Bg+OflL4LKzkjbXAULXvr3mYLs=
+github.com/halogenica/beautifulhugo v0.0.0-20260112152821-6173aa260601 h1:TgaiISjn8jN5jbK40fTvNafaznGDnSpgk+MsR/uqyJk=
+github.com/halogenica/beautifulhugo v0.0.0-20260112152821-6173aa260601/go.mod h1:4dwHt6njigk+fr9W3Bg+OflL4LKzkjbXAULXvr3mYLs=
```

## Local development

```sh
cd site
hugo serve
```
or
```sh
/run.sh
```

## Upload generated page to your hoster

Adapt the [copyUpstream.sh.example](https://github.com/voteeasy/webpage/blob/main/copyUpstream.sh.example) to your needs and run it afterwards.

## Known errors

## Permission denied for static assets

In case you experience this error message:
```sh
Error: error copying static files: open voteeasy/webpage/site/public/img/avatar-icon.png: permission denied
```
just rerun hugo serve multiple times until the message disappears.

## Theme questions / contributions

* [Typo in shell script](https://github.com/halogenica/beautifulhugo/pull/547)
* [Reference icons](https://github.com/halogenica/beautifulhugo/issues/549#issuecomment-3736990380)
* [Mailto in social sharing](https://github.com/halogenica/beautifulhugo/pull/550)
* Colourcode of the icon is '#ed9b57'
