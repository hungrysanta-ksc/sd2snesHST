# 출처와 고지

sd2snesHST 0.9.0은 GBC C44 실행 파일과 동일합니다. 고정 구현 커밋은 [35ef4ae](https://github.com/hungrysanta-ksc/fpga-cyclone4-game/tree/35ef4aef14fc6abef6495a980b7f00f257e5174f)입니다.

- **sd2snes**: MCU 및 보드 경로. 고정 커밋 `cf7e21d7a5978fcd74981d71c3cfbf6e982a4dd1`. GPL-2.0 및 개별 파일의 원래 조건을 유지합니다.
- **Gameboy_MiSTer / T80**: CPU·PPU·음향 기반. 고정 커밋 `7a5ff50528cd9c1d13ffb675e7df8506bffaa078`. gb.v의 GPL-3.0-or-later, T80의 개별 허용 조건과 고지를 유지합니다.
- **SameBoy / Lior Halphon**: 공개 CGB 부트 구현. MIT 고지를 유지합니다. 상용 SGB BIOS를 포함하지 않습니다.
- **Intel/Altera PLL wrapper**: 생성 소스의 원래 Intel/Altera 조건을 유지합니다.

자세한 변경 범위와 파일별 출처는 개발 저장소의 [의존성 등록부](https://github.com/hungrysanta-ksc/fpga-cyclone4-game/blob/35ef4aef14fc6abef6495a980b7f00f257e5174f/docs/DEPENDENCY-REGISTER.ko.md)와 소스 ZIP의 `source-manifest.json`을 참조하세요. 핵심 고지 원문은 업데이트 ZIP의 `licenses/`와 소스 ZIP에 포함합니다.

현재 저장소 전체에 새로운 단일 라이선스를 지정하지 않았습니다. 기존 파일의 라이선스는 계속 적용하며 자체 작성 부분과 개별 고지가 없는 upstream 파일의 배포 고지 범위는 공개 릴리스 전 검토 항목으로 남아 있습니다.
