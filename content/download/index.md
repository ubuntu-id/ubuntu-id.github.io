---
title: "Unduh Ubuntu"
description: "Anda dapat mengunduh versi terbaru Ubuntu dan menginstal serta menggunakannya di berbagai lingkungan."
image: "download.svg"
backgroundType: suru #light, dark, accent, suru, suru-topped, image
ubuntuVersions:
    ltsVersion: "26.04 LTS"
    normalVersion: "26.10"
    ltsReleaseNote: https://documentation.ubuntu.com/release-notes/26.04/
    normalReleaseNote: https://documentation.ubuntu.com/release-notes/26.10/
---

# Versi dan kebutuhan sistem
## Ubuntu {{< param "ubuntuVersions.ltsVersion" >}}
Ubuntu {{< param "ubuntuVersions.ltsVersion" >}}, versi LTS (Long Term Support) terbaru, mendapat pemeliharaan dan pembaruan keamanan gratis selama 5 tahun.
Untuk penggunaan yang stabil, versi LTS umumnya direkomendasikan.

[Lihat catatan rilis Ubuntu {{< param "ubuntuVersions.ltsVersion" >}}]({{< param "ubuntuVersions.ltsReleaseNote" >}})

## Ubuntu {{< param "ubuntuVersions.normalVersion" >}}
Jika ingin mencoba fitur terbaru, coba Ubuntu {{< param "ubuntuVersions.normalVersion" >}}, versi terbaru. Versi ini mendapat pemeliharaan dan pembaruan keamanan gratis selama 9 bulan.

[Lihat catatan rilis Ubuntu {{< param "ubuntuVersions.normalVersion" >}}]({{< param "ubuntuVersions.normalReleaseNote" >}})

## Siklus rilis dan dukungan Ubuntu
Versi baru Ubuntu dirilis setiap April dan Oktober, dengan jeda 6 bulan. Versi LTS baru dirilis setiap April tahun genap, dengan jeda 2 tahun.
Pemeliharaan dan pembaruan keamanan gratis diberikan selama 5 tahun untuk versi LTS dan 9 bulan untuk rilis sementara.
Informasi siklus rilis Ubuntu dapat dilihat di ubuntu.com.

{{< button text="Siklus rilis Ubuntu" href="https://ubuntu.com/about/release-cycle" icon="information" >}}

## Kebutuhan sistem

 - Prosesor dual core 2 GHz dan memori sistem 4 GB atau lebih baik
 - Ruang kosong hard disk 25 GB
 - Akses internet akan membantu
 - Drive DVD atau port USB untuk media instalasi

# Unduh

## Dari situs resmi

{{< button text="Desktop" href="https://ubuntu.com/download/desktop" icon="begin-downloading" >}}
{{< button text="Server" href="https://ubuntu.com/download/server" icon="machines" >}}
{{< button text="Raspberry Pi" href="https://ubuntu.com/download/raspberry-pi" icon="switcher-dashboard" >}}
{{< button text="Internet of Things (Ubuntu Core)" href="https://ubuntu.com/download/iot" icon="switcher-dashboard" >}}

## Dari mirror Indonesia
Anda dapat mengunduh image CD/DVD Desktop dan Server dari server mirror di Indonesia dengan kecepatan tinggi.

{{< button text="Jagoan Hosting" href="https://mirror.jagoanhosting.id/ubuntu-releases/" icon="begin-downloading" >}}
{{< button text="Citrahost" href="https://mirror.citrahost.com/ubuntu-releases/" icon="begin-downloading" >}}
{{< button text="Universitas Airlangga" href="https://mirror.unair.ac.id/ubuntu-cd/" icon="begin-downloading" >}}
{{< button text="Biznet Gio" href="https://mirror.biznetgio.com/ubuntu-cd/" icon="begin-downloading" >}}
{{< button text="Datautama" href="https://kartolo.sby.datautama.net.id/ubuntu-cd/" icon="begin-downloading" >}}
{{< button text="PENS (Politeknik Elektronika Negeri Surabaya)" href="https://kebo.pens.ac.id/ubuntu-cd/" icon="begin-downloading" >}}
{{< button text="EEPIS-ITS" href="http://kebo.vlsm.org/ubuntu-cd/" icon="begin-downloading" >}}

[Lihat daftar semua mirror arsip resmi Ubuntu di Launchpad.net](https://launchpad.net/ubuntu/+archivemirrors)

# Cara menginstal dan menggunakan

## Desktop & Server
- Desktop: [Panduan instalasi](https://wiki.ubuntu.com/index.php/Getting_Started), [Tutorial instalasi](https://ubuntu.com/tutorials/install-ubuntu-desktop)
- Server: [Tutorial instalasi](https://ubuntu.com/tutorials/install-ubuntu-server)
- [Daftar perangkat keras bersertifikat Ubuntu](https://ubuntu.com/certified)
## Penggunaan di cloud publik
- [Image cloud publik](https://cloud-images.ubuntu.com/)
- Amazon Web Services: [Marketplace](https://aws.amazon.com/marketplace/seller-profile?id=565feec9-3d43-413e-9760-c651546613f2), [Dokumentasi](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EC2_GetStarted.html)
- Microsoft Azure: [Ubuntu di Azure](https://azure.microsoft.com/en-us/ubuntu/#overview), [Dokumentasi](https://learn.microsoft.com/en-us/azure/virtual-machines/linux/quick-create-portal)
- Google Cloud Platform: [Marketplace](https://console.cloud.google.com/marketplace/product/ubuntu-os-cloud/ubuntu-focal), [Dokumentasi](https://cloud.google.com/sdk/docs/quickstart-debian-ubuntu)

## WSL (Windows Subsystem for Linux)
Jika memakai Windows 10 atau Windows 11 versi terbaru, Anda dapat mencoba Ubuntu dengan mudah lewat WSL.

{{< button text="Instal Ubuntu di WSL (dokumentasi WSL Indonesia User Group)" href="https://wslhub.com/wsl-firststep/firststep/install/" icon="begin-downloading" >}}

## Linux Containers

Image untuk Application Containers: untuk membangun image OCI yang dipakai dengan Docker, Podman, Kubernetes.

{{< button text="Docker Hub" href="https://hub.docker.com/_/ubuntu" icon="begin-downloading" >}}
{{< button text="Amazon ECR Public Gallery" href="https://gallery.ecr.aws/ubuntu/ubuntu" icon="begin-downloading" >}}

Image untuk System Containers (container bergaya VM): dipakai dengan LXD dan LXC sebagai pengganti beban kerja VM.

{{< button text="Lihat image container untuk LXD, LXC" href="https://uk.lxd.images.canonical.com/" icon="begin-downloading" >}}
{{< button text="linuxcontainers.org" href="https://linuxcontainers.org/" >}}

# Mendapatkan bantuan
Jika butuh bantuan saat memakai Ubuntu, Anda bisa bertanya di komunitas daring seperti forum dan obrolan.

{{< button text="Forum" href="https://forum.ubuntu-id.org/" >}}
{{< button text="Grup Facebook" href="https://www.facebook.com/groups/2327054593" >}}
{{< button text="Milis" href="https://groups.google.com/group/id-ubuntu/" >}}
{{< button text="Obrolan (Telegram, Facebook)" href="../chat" >}}

{{< button text="Ask Ubuntu" href="https://askubuntu.com/" >}}
{{< button text="Ubuntu Forums" href="https://ubuntuforums.org/" >}}
{{< button text="Launchpad Answers" href="https://answers.launchpad.net/ubuntu" >}}

# Dukungan teknis komersial

{{< info title="Catatan" content="Komunitas Ubuntu Indonesia adalah komunitas nirlaba yang terdiri dari pengguna dan pengembang, dan independen dari Canonical Ltd. Kami tidak menyediakan dukungan teknis komersial maupun jawaban atas pertanyaan terkait. Jika membutuhkan dukungan komersial untuk Ubuntu, lihat informasi di bawah dan dapatkan dukungan dari Canonical Ltd. atau mitra Canonical.">}}

## Ubuntu Advantage
Dapatkan dukungan teknis komersial dari Canonical Ltd., penerbit Ubuntu, lewat program Ubuntu Advantage.
Paket yang tersedia adalah Essential (gratis), Standard (berbayar), dan Advanced (berbayar). Anda bisa mendapat dukungan untuk Desktop, Server, VM, dan aplikasi (mis. MySQL, MongoDB, NGINX, Kafka, dan lainnya).


{{< button text="Ubuntu Advantage" href="https://ubuntu.com/advantage" icon="information" >}}

## Ubuntu Pro untuk cloud publik
Memakai AWS, Google Cloud, atau Microsoft Azure? Buat beban kerja VM dengan Ubuntu Pro, image Ubuntu premium dari Canonical Ltd., dan dapatkan dukungan teknis komersial tanpa kontrak tambahan.

{{< button text="Ubuntu Pro untuk AWS" href="https://ubuntu.com/aws/pro" icon="information" >}}
{{< button text="Ubuntu Pro untuk Azure" href="https://ubuntu.com/azure/pro" icon="information" >}}
{{< button text="Ubuntu Pro untuk Google Cloud" href="https://ubuntu.com/gcp/pro" icon="information" >}}

## Mitra Canonical
Mitra Canonical Ltd. juga menyediakan dukungan teknis komersial.

{{< button text="Cari mitra Canonical" href="https://canonical.com/partners/find-a-partner" icon="information" >}}
