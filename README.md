# sd2snesHST

**HungrySanTa의 FXPAK Pro 추가 코어 프로젝트**

sd2snesHST 는 FXPAK Pro 에서 GB/GBC를 비롯한 추가 게임 코어를 사용할 수 있도록 확장하는 프로젝트입니다.
구동환경 : sd2snes + FXPAK Pro / Mk.III, STM32 MCU + Cyclone IV EP4CE15F17C8
=> 즉 2026.10 시점 크리츠에서 판매중인 최신 에버드라이브 환경&사양에서 구동할 수 있는 모든 코어를 지원하는게 목표입니다.

비정기적으로 업데이트 되며 AI 에이전트를 적극 활용합니다.

> **0.9.0 최종 배포 자료 준비 완료.** 아래 Releases에서 공개된 버전을 확인하세요. 관리자 검토용 초안은 일반 사용자에게 보이지 않습니다.

## 다운로드와 설치

공개된 버전은 [Releases](https://github.com/hungrysanta-ksc/sd2snesHST/releases)에서 제공합니다. 설치용 파일은 `01-sd2snesHST-v0.9.0-update.zip`입니다. GitHub의 자동 생성 “Source code” ZIP은 설치 파일이 아닙니다.

**[설치·조작·저장·RTC 가이드](docs/USER-GUIDE.ko.md)** · [호환성과 지원 범위](docs/COMPATIBILITY.ko.md) · [변경 기록](CHANGELOG.md)

- 대상: **FXPAK Pro / Mk.III**, STM32 MCU + Cyclone IV EP4CE15F17C8.
- 정상 설치된 공식 sd2snes 1.11.2 계열에 추가하는 업데이트입니다. 빈 SD용 전체 펌웨어가 아닙니다.
- 전원을 끄고 기존 펌웨어·세이브·설정을 백업한 뒤 ZIP의 파일을 같은 폴더에 합쳐 복사합니다.
- 기존 RTC 시차 설정은 유지하세요. 동봉 `+540`은 한국/일본 현지 시각용입니다.
- 구형 SD2SNES/Mk.II 및 다른 포크와의 혼합 설치는 검증하지 않았습니다.
- 한줄 요약 : ZIP을 PC에 풀고 **그 안의 `sd2snes` 폴더를 SD 카드 루트의 기존 `sd2snes` 폴더에 합쳐 복사**하면 됩니다. `sd2snes/sd2snes`로 중첩되지 않게 해주세요.

## 0.9.0 의 기능

GB/GBC 게임 실행, SRAM 저장·자동 기록, MBC3 RTC, 강제 저장 4슬롯, 약 3배 빨리감기, 소리 설정과 게임 리셋을 제공합니다.
특히 그동안 SFC 에서 실행 불가능했던 GBC 전용 게임의 실행을 지원합니다.
게임 **복사본**의 확장자를 `.egbc`로 바꾸면 새 코어로 실행됩니다. `.gb`와 `.gbc`는 기존 SGB 경로이며 기존 SGB 파일이 필요합니다.

- **L + R + Start**: 코어 메뉴
- **R을 누르고 있기**: 빨리감기
- **WRITE SRAM**: 게임의 저장 RAM을 SD에 기록
- **SAVE STATE / LOAD STATE**: 현재 실행 상태를 저장·복원

게임 ROM·개인 세이브·SGB 코어·BIOS는 배포하지 않습니다. NES·PCE는 향후 조사 대상이며 0.9.0에는 포함하지 않습니다.

## 문제 보고와 개발

[문제 보고](https://github.com/hungrysanta-ksc/sd2snesHST/issues/new/choose)에는 제품 버전, 기기, 게임 이름·지역·패치 버전, 재현 순서와 증상을 적어 주세요. 일반 배포판은 진단 로그를 자동 생성하지 않습니다.

구현 소스와 개발 기록은 [개발 저장소](https://github.com/hungrysanta-ksc/fpga-cyclone4-game)에서 관리합니다. 릴리스의 `02-sd2snesHST-v0.9.0-source.zip`은 0.9.0 실행 소스와 필요한 MCU 원본·빌드 입력·라이선스·재현 지침을 담으며, 이 사용자 저장소의 자동 생성 소스 ZIP과 다릅니다.

[출처와 고지](THIRD-PARTY-NOTICES.md) · [0.9.0 파일·소스 대응표](manifests/0.9.0.json)
