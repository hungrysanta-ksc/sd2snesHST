# 변경 기록

## 0.9.0

Gameboy_MiSTer 기반 GB/GBC FPGA 코어를 FXPAK Pro에 이식한 첫 제품 버전입니다. 초기 구동에는 SameBoy 유래 공개 CGB 부트 코드를 사용합니다.

- `.egbc` GB/GBC 코어와 기존 `.gb` / `.gbc` SGB 경로 공존.
- SRAM 기록·자동 기록, MBC3 RTC 보존.
- 강제 저장·복원 4슬롯, R 버튼 약 3배 빨리감기.
- 코어 메뉴, 소리 설정, 게임 리셋.
- 로딩·캡처·상태 진단 파일 기록 비활성화. 게임 저장·설정은 계속 기록.
- 설치 가이드, 호환성 기록, 오프라인 준비가 가능한 대응 소스 ZIP, 구성별 라이선스 고지와 SHA256 체크섬 제공.

FXPAK Pro / Mk.III용 업데이트입니다. 지원 범위는 [호환성 기록](docs/COMPATIBILITY.ko.md)을 참조하세요.
