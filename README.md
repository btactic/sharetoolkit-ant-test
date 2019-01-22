# ShareToolkit extension built thanks to ant


This is a proof a concept in order to:

* Build any extension (ShareToolkit in this example) thanks to javac included with Zimbra
* And build against Zimbra jar binaries in a Zimbra installation

In this way you do not need to have your own jar libraries or build them from Zimbra source code.

This code works with ZCS 8.7 .

This repo is not meant to be used in production.

## Deployment of source code:

 Make sure the source code of this repo comes into:

```
/opt/zimbra/conf/scripts/sharetoolkit-test/
```

 with zimbra:zimbra permissions.

so that:

```
sudo su - zimbra
cd /opt/zimbra/conf/scripts/sharetoolkit-test/
ls
```

shows:

```
META-INF  build  build.xml  dist  src
```
.


## Build

```
sudo su - zimbra
cd /opt/zimbra/conf/scripts/sharetoolkit-test/
ant
```

## Outputs

JAR file will be found in:

```
dist/ShareToolkit.jar
```
.
