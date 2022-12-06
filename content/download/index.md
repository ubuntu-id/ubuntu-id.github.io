---
title: "우분투 Unduh"
description: "최신 버전의 우분투를 내려받아 다양한 환경에 설치하여 사용할 수 있습니다."
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

# 버전 및 요구사양
## 우분투 {{< param "ubuntuVersions.ltsVersion" >}}
가장 최근 출시된 LTS(장기 지원) 버전인 우분투 {{< param "ubuntuVersions.ltsVersion" >}}는 5년간 유지보수 및 보안 업데이트가 무료로 제공됩니다.
대부분의 경우, 안정적인 사용을 위해 LTS 버전 사용이 권장됩니다.

[우분투 {{< param "ubuntuVersions.ltsVersion" >}} 릴리즈 노트 보기(한국어 번역)]({{< param "ubuntuVersions.ltsReleaseNoteKor" >}})
[우분투 {{< param "ubuntuVersions.ltsVersion" >}} 릴리즈 노트 보기]({{< param "ubuntuVersions.ltsReleaseNote" >}})

## 우분투 {{< param "ubuntuVersions.normalVersion" >}}
새로운 기능을 먼저 사용해 보고 싶다면, 가장 최신 버전인 우분투 {{< param "ubuntuVersions.normalVersion" >}}를 사용해 보세요. 출시 후 9개월간 유지보수 및 보안 업데이트가 무료로 제공됩니다.

[우분투 {{< param "ubuntuVersions.normalVersion" >}} 릴리즈 노트 보기]({{< param "ubuntuVersions.normalReleaseNote" >}})

## 우분투 출시 및 지원 주기
우분투는 새 버전이 매년 4월과 10월, 6개월 간격으로 새로 출시되며. 짝수 년도 4월, 2년 간격으로 장기 지원(LTS) 버전이 출시됩니다.
장기 지원 버전은 5년간, 장기 지원 사이 출시되는 일번 버전은 9개월간 유지보수 및 보안 업데이트가 무료로 제공됩니다.
우분투 홈페이지에서 각 버전별 지원 주기를 확인하실 수 있습니다.

{{< button text="Ubuntu release cycle (영어)" href="https://ubuntu.com/about/release-cycle" icon="information" >}}

## 요구 사양

 - 최소 2GHz 듀얼 코어 프로세서와 4GB 시스템 메모리
 - 25GB 이상의 저장 장치 여유공간
 - 인터넷 연결은 있으면 좋습니다.
 - 설치 매체로 사용할 장치: DVD 드라이브, USB 디스크 등

# Unduh

## 공식 홈페이지에서 Unduh

{{< button text="데스크탑" href="https://ubuntu.com/download/desktop" icon="begin-downloading" >}}
{{< button text="서버" href="https://ubuntu.com/download/server" icon="machines" >}}
{{< button text="Raspberry Pi" href="https://ubuntu.com/download/raspberry-pi" icon="switcher-dashboard" >}}
{{< button text="사물인터넷 (Ubuntu Core)" href="https://ubuntu.com/download/iot" icon="switcher-dashboard" >}}

## 국내 미러 서버에서 Unduh
국내 미러 서버에서 데스크탑 또는 서버용 CD/DVD 이미지를 빠르게 내려받을 수 있습니다.

{{< button text="KAIST" href="http://ftp.kaist.ac.kr/ubuntu-cd/HEADER.html" icon="begin-downloading" >}}
{{< button text="카카오 (Kakao Corp.)" href="https://mirror.kakao.com/ubuntu-releases/" icon="begin-downloading" >}}
{{< button text="LANET" href="https://ftp.lanet.kr/ubuntu-releases/" icon="begin-downloading" >}}
{{< button text="AniGil Linux Archive" href="https://mirror.anigil.com/ubuntu-cd/HEADER.html" icon="begin-downloading" >}}
{{< button text="Harukasan (부경대학교)" href="https://ftp.harukasan.org/ubuntu-releases/HEADER.html" icon="begin-downloading" >}}
{{< button text="Misaka Mikoto Network Mirror" href="https://mirror.misakamikoto.network/ubuntu-releases/" icon="begin-downloading" >}}

[Launchpad.net 에서 모든 우분투 공식 미러 목록 보기](https://launchpad.net/ubuntu/+archivemirrors)

# 설치 및 사용하기

## 데스크탑 및 서버
- 데스크탑: [설치 가이드](http://wiki.ubuntu-kr.org/index.php/Getting_Started), [설치 튜토리얼(영어)](https://ubuntu.com/tutorials/install-ubuntu-desktop)
- 서버: [설치 튜토리얼(영어)](https://ubuntu.com/tutorials/install-ubuntu-server)
- [우분투 인증 하드웨어 목록](https://ubuntu.com/certified)
## 퍼블릭 클라우드에서 사용하기
- [퍼블릭 클라우드용 이미지](http://cloud-images.ubuntu.com/)
- Amazon Web Services: [마켓플레이스](https://aws.amazon.com/marketplace/seller-profile?id=565feec9-3d43-413e-9760-c651546613f2), [문서](https://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/EC2_GetStarted.html)
- Microsoft Azure: [Ubuntu on Azure](https://azure.microsoft.com/ko-kr/ubuntu/#overview), [문서](https://docs.microsoft.com/ko-kr/azure/virtual-machines/linux/quick-create-portal)
- Google Cloud Platform: [마켓플레이스](https://console.cloud.google.com/marketplace/product/ubuntu-os-cloud/ubuntu-focal), [문서](https://cloud.google.com/sdk/docs/quickstart-debian-ubuntu)

## WSL (Windows Subsystem for Linux)
최신 버전의 Windows 10 또는 Windows 11 을 사용 중이라면, WSL 환경으로 우분투를 편리하게 만나보실 수 있습니다.

{{< button text="WSL 환경에 우분투 설치 (WSL Korea User Group 문서)" href="https://wslhub.com/wsl-firststep/firststep/install/" icon="begin-downloading" >}}

## 리눅스 컨테이너(Linux Container)

애플리케이션 컨테이너 이미지: Docker, Podman, Kubernetes 등 OCI 규격 컨테이너 이미지 빌드에 사용합니다.

{{< button text="Docker Hub" href="https://hub.docker.com/_/ubuntu" icon="begin-downloading" >}}
{{< button text="Amazon ECR Public Gallery" href="https://gallery.ecr.aws/ubuntu/ubuntu" icon="begin-downloading" >}}

시스템 컨테이너 (VM 스타일 컨테이너) 이미지: LXD, LXC 에서 사용하며, 단순히 VM을 대체하는 용도의 컨테이너용으로 쓰이는 이미지 입니다.

{{< button text="LXD, LXC용 컨테이너 이미지 모두 보기" href="https://uk.lxd.images.canonical.com/" icon="begin-downloading" >}}
{{< button text="linuxcontainers.org" href="https://linuxcontainers.org/" >}}

# 도움 받기
사용 중 도움이 필요하시면, 포럼과 채팅 등 다양한 온라인 커뮤니티에서 도움을 받으실 수 있습니다.

{{< button text="포럼" href="https://forum.ubuntu-kr.org/" >}}
{{< button text="페이스북 그룹" href="https://fb.com/groups/ubuntu.ko" >}}
{{< button text="메일링 리스트" href="https://lists.ubuntu.com/archives/ubuntu-ko/" >}}
{{< button text="채팅 (Slack, IRC)" href="../chat" >}}

{{< button text="Ask Ubuntu (영어)" href="https://askubuntu.com/" >}}
{{< button text="Ubuntu Forums (영어)" href="https://ubuntuforums.org/" >}}
{{< button text="Launchpad Answers (영어)" href="https://answers.launchpad.net/ubuntu" >}}

# 상용 기술 지원

{{< info title="참고사항" content="우분투 한국 커뮤니티는 Canonical Ltd.와는 독립적으로 운영되는 사용자 및 개발자 커뮤니티이며 비영리 형태로 운영되고 있습니다. 우분투에 상용 기술 지원을 제공하지 않으며, 관련 문의 답변도 불가능 합니다. 필요하신 경우, 아래 정보를 참고하셔서 Canonical Ltd. 또는 국내/해외 Canonical Partner로 부터 상용 기술 지원을 제공 받으시기 바랍니다." >}}

## Ubuntu Advantage
우분투를 개발한 Canonical Ltd. 로 부터 Ubuntu Advantage 상용 기술 지원을 받으실 수 있습니다.  
무료로 제공되는 Essential 플랜 및 Standard, Advanced 유료 플랜이 있으며, 데스크탑, 서버, VM, 응용 프로그램(MySQL, MongoDB, NGINX, Kafka 등) 에 대한 기술 지원이 제공됩니다.

{{< button text="Ubuntu Advantage (영어)" href="https://ubuntu.com/advantage" icon="information" >}}

## 퍼블릭 클라우드용 Ubuntu Pro
AWS, Google Cloud, Microsoft Azure 사용시, Canonical Ltd. 에서 제공하는 Ubuntu Pro 유료 프리미엄 이미지로 VM 워크로드를 생성할 수 있으며, 별도 추가 계약 없이 상용 기술 지원을 받을 수 있습니다. 

{{< button text="Ubuntu Pro for AWS (영어)" href="https://ubuntu.com/aws/pro" icon="information" >}}
{{< button text="Ubuntu Pro for Azure (영어)" href="https://ubuntu.com/azure/pro" icon="information" >}}
{{< button text="Ubuntu Pro for Google Cloud (영어)" href="https://ubuntu.com/gcp/pro" icon="information" >}}
## Canonical Partner
Canonical Ltd.의 파트너사에서도 상용 기술 지원을 제공합니다.

{{< button text="Find a Canonical partner (영어)" href="https://canonical.com/partners/find-a-partner" icon="information" >}}
