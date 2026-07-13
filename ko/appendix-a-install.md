---
title: 입력기 설치
nav_order: 7
parent: 한국어
description: 풍수 입력법 설치 가이드 —— Rime + 풍수 schema
permalink: /ko/appendix-a-install/
---

{% include lang_switch.html %}

# 입력기 설치
{: .fs-8 }

## Rime 입력기 다운로드 및 설치

1. [Rime 공식 홈페이지](https://rime.im/download/)에서 시스템에 맞는 최신 버전의 Rime(소랑호 / Weasel)을 다운로드하여 설치한다.

## 풍수 입력법 설치

1. 풍수 입력법의 5개 파일을 Rime 설치 디렉터리(`…\Rime\weasel-0.14.3\data`)에 복사하여, 원본 파일을 덮어쓴다.

   기본 설치 디렉터리: `C:\Program Files\Rime\weasel-0.14.3\data`

   5개 파일:

   - `default.yaml` —— 입력법 기본 설정 파일
   - `weasel.yaml` —— 입력법 인터페이스 설정 파일
   - `geomancy.dict.yaml` —— 풍수 입력법 사전 파일 (157 000 표제어)
   - `geomancy.extended.dict.yaml` —— 사용자 자체 정의 사전 파일
   - `geomancy.schema.yaml` —— 풍수 입력법 기능 설정 파일

2. 「시작」 → 「소랑호 입력법」 → 「입력법 설정」을 누른다.

3. 「풍수형음」을 선택하고 「中」 버튼을 눌러 확정한다.

   ![입력법 설정](/assets/images/install-1.png)

4. 원하는 인터페이스 스타일을 선택하고 「中」 버튼을 눌러 확정한다.

   ![인터페이스 스타일](/assets/images/install-2.png)

5. <kbd>Ctrl</kbd> + <kbd>`</kbd>(왼쪽 위 모서리 키)를 동시에 누르고, 「풍수형음」을 선택하여 입력법 설정을 마친다.

   ![schema 전환](/assets/images/install-3.png)

6. <kbd>Ctrl</kbd> + <kbd>Shift</kbd> 또는 <kbd>Ctrl</kbd> + <kbd>Space</kbd>로 입력법을 켜고 끈다.

   더 자세한 사용 안내는 [Rime 공식 홈페이지](https://rime.im/)의 도움말을 참조한다.

## 언제든 병음으로 전환

어떤 글자나 단어의 입력 코드가 잊혔을 때, 언제든 (<kbd>`</kbd> + 병음)으로 입력할 수 있다.

![병음으로 전환](/assets/images/install-4.png)
