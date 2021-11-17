# deb-builder-packagecloud
![build](https://github.com/zlig/deb-builder-packagecloud/actions/workflows/main.yml/badge.svg)

## Overview

Build Debian .deb packages builder tool (using GitHub Actions) and upload to PackageCloud


## Repository

The artifacts from this project are uploaded as samples in the following Package Cloud repository: [debs](https://packagecloud.io/geldtech/debs)

## Usage

### Add repository to the list of available sources

```
curl -s https://packagecloud.io/install/repositories/geldtech/debs/script.deb.sh | sudo bash
```

### Manual instructions to add repository to the list of available sources

```
echo "deb https://packagecloud.io/install/repositories/geldtech/debs /" | sudo tee -a /etc/apt/sources.list.d/geldtech_debs.list
sudo apt-get update
```

### Install package

```
sudo apt install deb-builder-packagecloud
```
