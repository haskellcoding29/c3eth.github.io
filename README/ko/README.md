# Cardano Catalyst Community Eastern Townhall website
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->

## 개요

[English](/README/en/README.md) | [Tiếng Việt](/README/vi/README.md) | [Indonesia](/README/id/README.md) | [日本語](/README/ja/README.md) | [한국어](/README/ko/README.md)

이 저장소에는 Cardano Catalyst Community (C3) Eastern Townhall (ETH)의 업데이트와 관련된 문서가 포함되어 있습니다. C3ETH 동부 시간대에 다양한 국가 및 언어 커뮤니티 구성원을 지원하고 있습니다. 팀의 중요한 초점은 Cardano Catalyst의 콘텐츠 및 온보딩을 지역화하고 가능한한 폭 넓은 참여를 가능하게 하는 것입니다.

이 저장소에는 Project Catalyst 문서, 커뮤니티 소스의 문서 및 관련된 제안 C3ETH에 의한 번역이 포함되어 있습니다. 콘텐츠는 동반구의 많은 언어로 번역되어 있으며, 특히 동아시아 언어에 초점이 맞춰져 있습니다.

[Project Catalyst](https://cardano.ideascale.com/)는 카르다노에 온체인 거버넌스를 도입하는 **시작**입니다. 카르다노 생태계의 미래 방향과 발전을 결정하기 위해 카탈리스트 커뮤니티의 집단 지성을 활용하는 일련의 실험입니다. 일련의 혁신을 위한 기금을 통해 커뮤니티는 어떤 아이디어에 자금을 조달할 것인지를 결정하고 제공합니다. 글로벌 블록체인 구축을 위한 최고의 아이디어를 조달할 것입니다.

## 도커를 이용한 빌드

웹사이트와 문서는 [Hugo](https://gohugo.io/)와 [Docsy Theme](https://www.docsy.dev/)를 사용하여 컴파일 및 개발되고 있습니다. 사이트를 구축하려면 [Node](https://nodejs.org/en/), [Npm](https://www.npmjs.com/) 및 [PostCSS](https://postcss.org/)가 필요합니다. ). 이러한 도구를 로컬에 설치하는 대신 [Docker](https://docs.docker.com/get-started/overview/)를 사용하여 사이트를 구축할 수 있습니다. 균일한 개발 환경을 제공할 수 있다는 장점이 있습니다.

- 도커: 도커를 설치하려면 [https://docs.docker.com/get-docker/](https://docs.docker.com/get-docker/) 문서를 참고하세요.

- 사이트 리포지토리의 작업 복사본(아래 참조)을 만든 후 리포지토리 루트 폴더에서 도커로 휴고 서브 컨테이너를 실행합니다:

  ```
  $ make container-serve
  ```

그런 다음 http://localhost:1313을 방문하여 설명서 사이트를 봅니다.

## 로컬 개발 환경으로 구축 

The Website is built using [Docsy](https://www.docsy.dev/) which is a [Hugo](https://gohugo.io/) theme for technical documentation sets, providing simple navigation, site structure, and more.
이 웹사이트는 기술문서 세트의 [Hugo](https://gohugo.io/) 테마인 [Docsy](https://www.docsy.dev/)를 사용하여 구축되어 간단한 탐색, 사이트 구조 등을 제공합니다.

### 전제조건

사이트를 로컬에서 구축하고 실행하려면 [Hugo](https://gohugo.io)의 'extended'버전이 필요합니다. 다음은 이 사이트를 구축하기 위한 기본 전제 조건입니다.

- Hugo "확장" 버전의 최신 릴리스를 설치합니다(버전 0.53 이상 권장). 
   [릴리스 페이지](https://github.com/gohugoio/hugo/releases)에서 설치하는 경우는 `_extended` 버전을 다운로드해야 합니다.
   SCSS를 지원합니다.

- 사이트 빌드에서 최종 CSS 자산을 생성할 수 있도록 'PostCSS'를 설치합니다. 프로젝트의 루트 디렉터리에서 다음 명령을 실행하여 로컬에 설치할 수 있습니다:

  ```
  sudo npm install -D --save autoprefixer
  sudo npm install -D --save postcss-cli
  ```

- 사이트 repo의 작업 복사본(아래 참조)을 만든 후에는 repo 루트 폴더에서 다음을 실행합니다:

  ```
  hugo server
  ```

## 웹사이트 복사

```bash
$ git clone --recurse-submodules --depth 1 https://github.com/c3eth/ce3th.github.io
$ cd c3eth.github.io
```

이 사이트는 하위 모듈로서 [Docsy 테마](https://www.docsy.dev/)에 기초하여 구축되어 있습니다. 하위 모듈을 업데이트하려면 다음을 실행하세요:

```bash
$ git submodule update --recursive
$ git pull --recurse-submodules
```
## 웹사이트 문서를 편집하기

문서는 ```content/{en,vn,in,jp,ko}``` 디렉토리에 있습니다. 편집이나 추가할 섹션을 선택하세요. 콘텐츠 구성에 대해서는 https://gohugo.io/content-management/organization/를 참조하세요. 

## 로그 변경

주목해야할 변경 및 버전에 대해서는 [CHANGELOG.md](CHANGELOG.md)를 참고로 하세요.

## 감사의 말

* [Project Catalyst](https://cardano.ideascale.com/)
* [Cardano Foundation](https://cardanofoundation.org/)
* [IOHK Project Catalyst Team](https://iohk.io/) 
* [Hugo](https://gohugo.io/)
* [Docsy](https://www.docsy.dev/)


## 기여하는 방법 ![GitHub](https://img.shields.io/github/contributors/c3eth/c3eth.github.io)

행동규칙과 풀요청을 제출하는 절차에 대해서 자세한 내용은 [CONTRIBUTING.md](https://github.com/c3eth/c3eth.github.io/blob/main/CONTRIBUTING.md)를 참조하세요.

이 프로젝트에 참여한 [기여자](https://github.com/c3eth/c3eth.github.io/graphs/contributors) 목록도 참조하세요.

이러한 훌륭한 기여자들에게 감사드립니다([그림문자](https://allcontributors.org/docs/en/emoji-key)를 참조):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

이 프로젝트는 [모든 기여자](https://github.com/all-contributors/all-contributors)의 사양을 따릅니다. 어떤 종류의 기여도 환영합니다!

## 라이센스 ![GitHub](https://img.shields.io/github/license/c3eth/c3eth.github.io)

저장소`c3eth / c3eth.github.io`에서 공개된 소스 코드는 Apache License 2.0하에 라이센스되어 있습니다. 자세한 내용은 [LICENSE (https://github.com/c3eth/c3eth.github.io/main/LICENSE.md) 파일을 참조하세요.

저장소`c3eth / c3eth.github.io`에 공개되어 있는 내용은 [Creative Attribution-Non-Commercial-ShareAlike (CC BY-NC-SA) License v4.0] (https://creativecommons.org/licenses/by -nc-sa / 4.0 /)하에 라이센스되어 있습니다.

소재를 임의의 매체나 형식으로 자유롭게 공유(복사, 재배포) 할 수 있고, 본 제품의 적응, 리믹스, 변환 및 구축을 할 수 있습니다. 아 자료를 영리 목적으로 사용할 수는 없습니다. 본 제품을 리믹스 변환 구축하는 경우는 원본과 같은 라이선스하에 배포해야 합니다. 보증은 없습니다. 라이센스는 의도된 사용에 필요한 모든 권한을 부여하지는 않습니다.
