# sd2snesHST 0.9.1

- 8 MiB MBC5 ROM 로딩을 지원합니다. 원피스 한국어판의 실행·플레이와 다른 8 MiB ROM의 실행을 실기에서 확인했습니다.
- Galaga: Destination Earth (USA)에서 두 로고 뒤 타이틀이 검게 나오던 문제를 수정했습니다.
- 해리 포터와 마법사의 돌 (v010)에서 폴리오마기의 ‘보호 → 괴짜 웬델린’ 카드가 표시되지 않던 문제를 수정했습니다. 두 게임의 문제 장면을 원래 RGB555 색으로 표시하며 실기에서 정상 동작을 확인했습니다.

## 설치
- FXPAK Pro / Mk.III 의 정상 설치된 공식 sd2snes 1.11.2 폴더 구조에 적용합니다.
- 본체 전원을 끄고 기존 SD를 백업한 뒤, `01-sd2snesHST-v0.9.1-update.zip`의 압축을 풀어 그 안의 `sd2snes` 폴더에 있는 4개 파일을 SD 카드의 기존 `sd2snes` 폴더에 합쳐 복사하세요. RTC 시차 파일은 아래 안내에 따라 기존 설정을 유지합니다.
- 동봉 RTC 시차는 한국/일본용 +540이며 기존 사용자 설정이 맞으면 유지합니다.

[사용 가이드](https://github.com/hungrysanta-ksc/sd2snesHST/blob/master/docs/USER-GUIDE.ko.md) · [호환성](https://github.com/hungrysanta-ksc/sd2snesHST/blob/master/docs/COMPATIBILITY.ko.md)

## 파일 설명
- **01-sd2snesHST-v0.9.1-update.zip**: 설치용 업데이트와 사용 가이드.
- **02-sd2snesHST-v0.9.1-source.zip**: 0.9.1 실행 소스·고정 MCU 원본·mini FPGA·CGB 부트 빌드 입력과 라이선스.
- **03-sd2snesHST-v0.9.1-manifest.json**: 대상 보드·소스·실행 파일·ZIP의 대응 관계.
- **04-SHA256SUMS.txt**: 위 3개 파일의 SHA256.

GitHub 자동 생성 Source code ZIP은 사용자 안내 저장소의 사본이며 펌웨어 소스 묶음이 아닙니다.

## 기능과 사용방법
- Gameboy_MiSTer 기반 코어로 GB 및 GBC 전용 게임을 실행합니다. SameBoy 유래 CGB 부트 코드가 초기 구동을 담당합니다.
- 새 코어로 실행할 게임은 **복사본**의 확장자를 `.egbc`로 바꿔 넣으세요. (`.gb`, `.gbc`는 기존 SGB 코어로 실행됩니다.)
- L+R+Start 로 코어 메뉴를 열 수 있습니다.
- 게임 내 저장 후 SRAM을 SD에 자동 기록합니다. (AUTO WRITE SRAM이 켜져 있어야 하며, 변경 감지 후 기록까지 지연이 있습니다. 전원을 끄기 전 확실히 기록하려면 WRITE SRAM을 실행하고 SAVED를 확인하세요.)
- MBC3 RTC를 지원합니다. (포켓몬 금·은 등의 시간 기능. FXPAK의 날짜·시각을 기준으로 전원이 꺼져 있던 동안의 경과 시간도 반영하므로 기기 시계와 RTC 시차를 맞춰 주세요.)
- R 버튼 누르고 있는걸로 약 3배 빨리감기가 동작합니다. (리버스는 지원되지 않습니다.)

기존 .gb/.gbc는 SGB 경로를 사용합니다. SGB 코어·BIOS·게임·개인 세이브는 포함하지 않습니다.

## 코어 메뉴설명
- SRAM 수동 쓰기와 자동쓰기 on/off 가 지원됩니다.
- 강제 세이브, 로드 기능이 구현되어 있으며 4슬롯을 지원합니다.
- 뮤트 설정이 가능합니다.
- 소프트웨어 리셋을 제공합니다.

## 검증
실행 파일·설정 파일과 대응 소스의 SHA256을 검증했습니다. 소스 ZIP의 MCU 오프라인 준비 및 원본 손상 거부 검사를 통과했습니다.

[출처와 라이선스](https://github.com/hungrysanta-ksc/sd2snesHST/blob/master/THIRD-PARTY-NOTICES.md)
