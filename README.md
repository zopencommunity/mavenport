[![Automatic version updates](https://github.com/ZOSOpenTools/mavenport/actions/workflows/bump.yml/badge.svg)](https://github.com/ZOSOpenTools/mavenport/actions/workflows/bump.yml)

# Maven

A build automation tool

# Installation and Usage

Use the zopen package manager ([QuickStart Guide](https://zopen.community/#/Guides/QuickStart)) to install:
```bash
zopen install maven
```

# Building from Source

1. Clone the repository:
```bash
git clone https://github.com/zopencommunity/mavenport.git
cd mavenport
```
2. Build using zopen:
```bash
zopen build -vv
```

See the [zopen porting guide](https://zopen.community/#/Guides/Porting) for more details.

# Documentation
Tip from a maven user:  
If you tag your `pom.xml` files with `ISO8859-1`, then `maven-install-plugin` will copy that file to the `.m2` cache, converting it to `IBM-1047` and `mvn deploy` will fail with a `409`.  
Tag your files UTF-8 and DO NOT set `_BPXK_AUTOCVT=MUST`.

# Troubleshooting
TBD

# Contributing
Contributions are welcome! Please follow the [zopen contribution guidelines](https://github.com/zopencommunity/meta/blob/main/CONTRIBUTING.md).
