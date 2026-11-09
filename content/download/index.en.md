---
title: "Download Ubuntu"
description: "Get latest version of Ubuntu and install it on various environments."
image: "download.svg"
backgroundType: suru #light, dark, accent, suru, suru-topped, image
ubuntuVersions:
    ltsVersion: "26.04 LTS"
    normalVersion: "26.10"
    ltsReleaseNote: https://documentation.ubuntu.com/release-notes/26.04/
    normalReleaseNote: https://documentation.ubuntu.com/release-notes/26.10/
---

# Version and system requirements
## Ubuntu {{< param "ubuntuVersions.ltsVersion" >}}
Ubuntu {{< param "ubuntuVersions.ltsVersion" >}}, the latest LTS(Long term support) version provides 5 years of maintenance and security updates for free.
In most cases, LTS version is recommended for stable use.

[See Ubuntu {{< param "ubuntuVersions.ltsVersion" >}} release notes]({{< param "ubuntuVersions.ltsReleaseNote" >}})

## Ubuntu {{< param "ubuntuVersions.normalVersion" >}}
If you want to try out latest features, Try out Ubuntu {{< param "ubuntuVersions.normalVersion" >}}, the latest version. It provides 9 months of maintenance and security updates for free.

[See Ubuntu {{< param "ubuntuVersions.normalVersion" >}} release notes]({{< param "ubuntuVersions.normalReleaseNote" >}})

## Ubuntu release and support cycle
New version of Ubuntu is released on every April and October with 6 months interval. And the new LTS version is released on April of even years with 2 years interval.
Free maintenance and security updates are provided 5 years for LTS version and 9 months for interim releases.
You may check out Ubuntu release cycle information on ubuntu.com

{{< button text="Ubuntu release cycle" href="https://ubuntu.com/about/release-cycle" icon="information" >}}

## System requirements

 - 2 GHz dual core processor and 4 GB system memory or better
 - 25 GB of free hard drive space
 - Internet access is helpful
 - Either a DVD drive or a USB port for the installer media

# Download

## From official website

{{< button text="Desktop" href="https://ubuntu.com/download/desktop" icon="begin-downloading" >}}
{{< button text="Server" href="https://ubuntu.com/download/server" icon="machines" >}}
{{< button text="Raspberry Pi" href="https://ubuntu.com/download/raspberry-pi" icon="switcher-dashboard" >}}
{{< button text="Internet of Things (Ubuntu Core)" href="https://ubuntu.com/download/iot" icon="switcher-dashboard" >}}

## From Indonesian Mirrors
You can download Desktop and Server CD/DVD images from Indonesian Mirror servers with fast speed.

{{< button text="Jagoan Hosting" href="https://mirror.jagoanhosting.id/ubuntu-releases/" icon="begin-downloading" >}}
{{< button text="Citrahost" href="https://mirror.citrahost.com/ubuntu-releases/" icon="begin-downloading" >}}
{{< button text="Universitas Airlangga" href="https://mirror.unair.ac.id/ubuntu-cd/" icon="begin-downloading" >}}
{{< button text="Biznet Gio" href="https://mirror.biznetgio.com/ubuntu-cd/" icon="begin-downloading" >}}
{{< button text="Datautama" href="https://kartolo.sby.datautama.net.id/ubuntu-cd/" icon="begin-downloading" >}}
{{< button text="PENS (Politeknik Elektronika Negeri Surabaya)" href="https://kebo.pens.ac.id/ubuntu-cd/" icon="begin-downloading" >}}
{{< button text="EEPIS-ITS" href="http://kebo.vlsm.org/ubuntu-cd/" icon="begin-downloading" >}}

[See list of All Official Archive Mirrors for Ubuntu on Launchpad.net](https://launchpad.net/ubuntu/+archivemirrors)

# How to install and use

## Desktop & Server
- Desktop: [Installation guide (Indonesian)](https://wiki.ubuntu.com/index.php/Getting_Started), [Installation tutorial](https://ubuntu.com/tutorials/install-ubuntu-desktop)
- Server: [Installation tutorial](https://ubuntu.com/tutorials/install-ubuntu-server)
- [List of Certified Ubuntu hardwares](https://ubuntu.com/certified)
## Use on Public Clouds
- [Public cloud images](https://cloud-images.ubuntu.com/)
- Amazon Web Services: [Marketplace](https://aws.amazon.com/marketplace/seller-profile?id=565feec9-3d43-413e-9760-c651546613f2), [Documentations](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EC2_GetStarted.html)
- Microsoft Azure: [Ubuntu on Azure](https://azure.microsoft.com/en-us/ubuntu/#overview), [Documentations](https://learn.microsoft.com/en-us/azure/virtual-machines/linux/quick-create-portal)
- Google Cloud Platform: [Marketplace](https://console.cloud.google.com/marketplace/product/ubuntu-os-cloud/ubuntu-focal), [Documentations](https://cloud.google.com/sdk/docs/quickstart-debian-ubuntu)

## WSL (Windows Subsystem for Linux)
If you are using latest version of Windows 10 or Windows 11, You can easily try out Ubuntu with WSL environment. 

{{< button text="Install Ubuntu on WSL (WSL Indonesia User Group Documentations)" href="https://wslhub.com/wsl-firststep/firststep/install/" icon="begin-downloading" >}}

## Linux Containers

Images for Application Containers: For building OCI images to use with Docker, Podman, Kubernetes.

{{< button text="Docker Hub" href="https://hub.docker.com/_/ubuntu" icon="begin-downloading" >}}
{{< button text="Amazon ECR Public Gallery" href="https://gallery.ecr.aws/ubuntu/ubuntu" icon="begin-downloading" >}}

Images for System Containers (VM Style Containers): Used with LXD and LXC for replacement of VM workloads.

{{< button text="See Container images for LXD, LXC" href="https://uk.lxd.images.canonical.com/" icon="begin-downloading" >}}
{{< button text="linuxcontainers.org" href="https://linuxcontainers.org/" >}}

# Get help
If you need help while using, You can get help on online community such as forums and online chat.

{{< button text="Ubuntu Discourse" href="https://discourse.ubuntu.com/" >}}
{{< button text="Facebook Group (Indonesian)" href="https://www.facebook.com/groups/2327054593" >}}
{{< button text="Mailing List (Indonesian)" href="https://groups.google.com/group/id-ubuntu/" >}}
{{< button text="Chat (Telegram, Facebook)" href="../chat" >}}

{{< button text="Ask Ubuntu" href="https://askubuntu.com/" >}}
{{< button text="Ubuntu Forums" href="https://ubuntuforums.org/" >}}
{{< button text="Launchpad Answers" href="https://answers.launchpad.net/ubuntu" >}}

# Commercial technical support

{{< info title="Note" content="Ubuntu Indonesia Community is a non-profit community consists of users and developers and independent from Canonical Ltd. We do not provide any commercial technical support and answers for related inqueires. If you need commercial support for Ubuntu, Check out informations below and get support from Canonical Ltd. or Canonical Partners.">}}

## Ubuntu Advantage
Get commercial technical support from Canonical Ltd. the publisher of Ubuntu with Ubuntu Advantage program.
Available plans are Essential(Free), Standard(Paid) and Advanced(Paid). You can get support for Desktops, Servers, VMs and applications(e.g. MySQL, MongoDB, NGINX, Kafka and more).


{{< button text="Ubuntu Advantage" href="https://ubuntu.com/advantage" icon="information" >}}

## Ubuntu Pro for Public Clouds
Using AWS, Google Cloud, Microsoft Azure? Create VM workloads with Ubuntu Pro, a premium Ubuntu image from Canonical Ltd. and get commercial technical support without additional contracts.

{{< button text="Ubuntu Pro for AWS" href="https://ubuntu.com/aws/pro" icon="information" >}}
{{< button text="Ubuntu Pro for Azure" href="https://ubuntu.com/azure/pro" icon="information" >}}
{{< button text="Ubuntu Pro for Google Cloud" href="https://ubuntu.com/gcp/pro" icon="information" >}}

## Canonical Partner
Partners of Canonical Ltd. also provides commercial technical supports.

{{< button text="Find a Canonical partner" href="https://canonical.com/partners/find-a-partner" icon="information" >}}
