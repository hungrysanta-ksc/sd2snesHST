# 출처와 라이선스

sd2snesHST 0.9.0의 구성별 출처와 라이선스입니다.

## HungrySanTa 자체 작성 부분

2026-10-04 소유자 승인에 따라 FPGA 통합 코드는 GPL-3.0-or-later, MCU 코드는 GPL-2.0-only, 독립 도구·렌더러 생성기·문서는 MIT로 제공합니다. 이 사용자 안내 저장소의 자체 문서는 [MIT](LICENSE)를 따릅니다. 원본 파일의 고지와 권리는 유지합니다.

## 사용한 프로젝트

| 구성 | 원본 기준과 고지 |
| --- | --- |
| sd2snes MCU·mini FPGA | cf7e21d7a5978fcd74981d71c3cfbf6e982a4dd1. GPLv2 및 파일별 기존 고지 유지. MCU의 GPL-2.0-only 표기를 유지합니다. |
| Gameboy_MiSTer | 7a5ff50528cd9c1d13ffb675e7df8506bffaa078. gb.v 등 GPL-3.0-or-later 표시와 나머지 원본 고지·출처를 유지합니다. |
| T80 | Daniel Wallner 등의 source/synthesized-form 재배포 조건과 저작권 고지 유지. |
| SameBoy CGB 부트 | Lior Halphon의 MIT 고지 유지. 상용 BIOS가 아닙니다. |
| Intel/Altera 생성 소스 | PLL 등 원래의 Intel/Altera 조건을 유지합니다. 대상 FPGA는 Intel Cyclone IV입니다. |

핵심 라이선스 원문은 설치 ZIP의 licenses/에, 각 소스의 원래 헤더와 파일별 출처는 source ZIP에 보존합니다. 개별 헤더가 없는 원본 파일을 자체 작성물로 간주하거나 새 라이선스로 덮지 않습니다.

## 대응 소스

- 대응 소스·고지·도구 기준: a2b1fb59390a96f70bbc8588a63e465831e7e247.
- source ZIP에 실행 소스, 고정 MCU 기본 소스·mini FPGA 입력, CGB 부트 입력, 해시 목록과 빌드 지침을 함께 제공합니다.
- source ZIP의 docs/SOURCE-BUNDLE.ko.md와 LICENSE.md가 정확한 범위와 재현 방법을 설명합니다.

[개발 소스와 고지](https://github.com/hungrysanta-ksc/fpga-cyclone4-game/tree/a2b1fb59390a96f70bbc8588a63e465831e7e247)
