---
title: "Download Ubuntu"
description: "Get latest version of Ubuntu and install it on various environments."
image: "download.svg"
backgroundType: suru #light, dark, accent, suru, suru-topped, image
ubuntuVersions:
    ltsVersion: "22.04 LTS"
    normalVersion: "21.10"
    ltsReleaseNoteKor: https://blog.ubuntu-kr.org/2022/04/22/jamme-jellyfish-release-notes/
    ltsReleaseNote: https://discourse.ubuntu.com/t/jammy-jellyfish-release-notes/24668
    normalReleaseNote: https://discourse.ubuntu.com/t/impish-indri-release-notes/21951
mirrors:
   - name: 
     url: https://ftp.harukasan.org/ubuntu-releases/HEADER.html
---

# Version and system requirements
## Ubuntu {{< param "ubuntuVersions.ltsVersion" >}}
Ubuntu {{< param "ubuntuVersions.ltsVersion" >}}, the latest LTS(Long term support) version provides 5 years of maintenance and security updates for free.
In most cases, LTS version is recommended for stable use.

[See Ubuntu {{< param "ubuntuVersions.ltsVersion" >}} release notes (Indonesian translation)]({{< param "ubuntuVersions.ltsReleaseNoteKor" >}})
[See Ubuntu {{< param "ubuntuVersions.ltsVersion" >}} release notes]({{< param "ubuntuVersions.ltsReleaseNote" >}})

## Ubuntu {{< param "ubuntuVersions.normalVersion" >}}
If you want to try out latest features, Try out Ubuntu {{< param "ubuntuVersions.normalVersion" >}}, the latest version. It provides 9 months of maintenance and security updates for free.

[See Ubuntu {{< param "ubuntuVersions.normalVersion" >}} release notes]({{< param "ubuntuVersions.normalReleaseNote" >}})

## Ubuntu release and support cycle
New version of Ubuntu is released on every April and October with 6 months interval. And the new LTS version is released on April of even years with 2 years interval.
Free maintenance and security updates are provided 5 years for LTS version and 9 months for interim releases.
You may check out Ubuntu release cycle information on ubuntu.com

{{< button text="Ubuntu release cycle (영어)" href="https://ubuntu.com/about/release-cycle" icon="information" >}}

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

## From Indonesia Mirrors
You can download Desktop and Server CD/DVD images from Indonesian Mirror servers with fast speed.

{{< button text="KAIST" href="http://ftp.kaist.ac.kr/ubuntu-cd/HEADER.html" icon="begin-downloading" >}}
{{< button text="Kakao Corp." href="https://mirror.kakao.com/ubuntu-releases/" icon="begin-downloading" >}}
{{< button text="LANET" href="https://ftp.lanet.kr/ubuntu-releases/" icon="begin-downloading" >}}
{{< button text="AniGil Linux Archive" href="https://mirror.anigil.com/ubuntu-cd/HEADER.html" icon="begin-downloading" >}}
{{< button text="Harukasan (Pukyong University)" href="https://ftp.harukasan.org/ubuntu-releases/HEADER.html" icon="begin-downloading" >}}
{{< button text="Misaka Mikoto Network Mirror" href="https://mirror.misakamikoto.network/ubuntu-releases/" icon="begin-downloading" >}}

[See list of All Official Archive Mirrors for Ubuntu on Launchpad.net](https://launchpad.net/ubuntu/+archivemirrors)

# How to install and use

## Desktop & Server
- Desktop: [Installation guide (Indonesian)](http://wiki.ubuntu-kr.org/index.php/Getting_Started), [Installation tutorial](https://ubuntu.com/tutorials/install-ubuntu-desktop)
- Server: [Installation tutorial](https://ubuntu.com/tutorials/install-ubuntu-server)
- [List of Certified Ubuntu hardwares](https://ubuntu.com/certified)
## Use on Public Clouds
- [Public cloud images](http://cloud-images.ubuntu.com/)
- Amazon Web Services: [Marketplace](https://aws.amazon.com/marketplace/seller-profile?id=565feec9-3d43-413e-9760-c651546613f2), [Documentations](https://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/EC2_GetStarted.html)
- Microsoft Azure: [Ubuntu on Azure](https://azure.microsoft.com/ko-kr/ubuntu/#overview), [Documentations](https://docs.microsoft.com/ko-kr/azure/virtual-machines/linux/quick-create-portal)
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

{{< button text="Forums (Indonesian)" href="https://forum.ubuntu-kr.org/" >}}
{{< button text="Facebook Group (Indonesian)" href="https://fb.com/groups/ubuntu.ko" >}}
{{< button text="Mailing List (Indonesian)" href="https://lists.ubuntu.com/archives/ubuntu-ko/" >}}
{{< button text="Chat (Slack, IRC)" href="../chat" >}}

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
