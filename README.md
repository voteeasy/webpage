# webpage

This project contains the webpage of VoteEasy published at https://voteeasy.aiki-it.de

<img src="https://img.shields.io/liberapay/receives/ottlinger.svg?logo=liberapay">

## External references / resources

* Theme: https://github.com/halogenica/beautifulhugo
* Example: https://hugo-theme-beautifulhugo.netlify.app/
* CMS/Hugo: https://gohugo.io/getting-started/quick-start/

## Hugo installation

Get a recent version, such as

```sh
$ hugo version
hugo v0.152.2-6abdacad3f3fe944ea42177844469139e81feda6+extended
linux/amd64 BuildDate=2025-10-24T15:31:49Z VendorInfo=snap:0.152.2
```

## Mac installation

As the theme is installed as a hugo module you may run into an error message if there's no go available:

```
Error: command error:
failed to load modules: failed to download modules: failed to execute 'go [mod download]':
failed to execute binary "go" with args [mod download]: go: go.mod requires go >= 1.25.5 (running go 1.25.3)
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

In case you installed as hugo module got to the site-subfolder and:

```sh
$ hugo mod get
```

or use the convenience helper script in this project's basefolder:

```sh
$ ./updateTheme.sh
```
 
Download starts and you will get a diff such as:

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
to also get Git information into the pages.

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

### Merge requests

* [Typo in shell script](https://github.com/halogenica/beautifulhugo/pull/547)
* [Reference icons](https://github.com/halogenica/beautifulhugo/issues/549#issuecomment-3736990380)
* [Mailto in social sharing](https://github.com/halogenica/beautifulhugo/pull/550)
* [German translation errors](https://github.com/halogenica/beautifulhugo/pull/551)
* Colour code of the icon is `#ed9b57`
* [GitPageInfo contains wrong date](https://github.com/halogenica/beautifulhugo/issues/552)
* [Handle singular/plural values in reading time](https://github.com/halogenica/beautifulhugo/pull/553), adapt [en](https://github.com/halogenica/beautifulhugo/pull/554) default as well

### Questions / discussions
* Question: [allow ASCII-encoding of mail addresses](https://github.com/halogenica/beautifulhugo/issues/548)
