# sd2snesHST 0.9.0

HungrySanTa의 FXPAK Pro 추가 코어 프로젝트 첫 릴리스입니다.

## 설치
FXPAK Pro / Mk.III의 정상 설치된 공식 sd2snes 1.11.2 계열 위에 적용합니다. 기존 SD를 백업하고 업데이트 ZIP의 파일을 합쳐 복사하세요. 동봉 RTC 시차는 한국/일본용 +540이며 기존 사용자 설정이 맞으면 유지합니다.

[사용 가이드](https://github.com/hungrysanta-ksc/sd2snesHST/blob/master/docs/USER-GUIDE.ko.md) · [호환성](https://github.com/hungrysanta-ksc/sd2snesHST/blob/master/docs/COMPATIBILITY.ko.md)

## 파일 선택
- **01-sd2snesHST-v0.9.0-update.zip**: 설치용 업데이트와 사용 가이드.
- **02-sd2snesHST-v0.9.0-source.zip**: 0.9.0 실행 소스·고정 MCU 원본·mini FPGA·CGB 부트 빌드 입력과 라이선스.
- **03-sd2snesHST-v0.9.0-manifest.json**: 대상 보드·소스·실행 파일·ZIP의 대응 관계.
- **04-SHA256SUMS.txt**: 위 3개 파일의 SHA256.

GitHub 자동 생성 Source code ZIP은 사용자 안내 저장소의 사본이며 펌웨어 소스 묶음이 아닙니다.

## 기능과 범위
.egbc GB/GBC 코어, SRAM·자동 기록, MBC3 RTC, 강제 저장 4슬롯, R 버튼 약 3배 빨리감기, 소리 설정, 게임 리셋을 제공합니다. load/cap/state 진단 로그는 생성하지 않습니다.

기존 .gb/.gbc는 SGB 경로를 사용합니다. SGB 코어·BIOS·게임·개인 세이브는 포함하지 않습니다. NES·PCE는 이번 버전에 포함하지 않습니다.

## 검증
실행 파일·설정 파일과 대응 소스의 SHA256을 검증했습니다. 소스 ZIP의 MCU 오프라인 준비 및 원본 손상 거부 검사를 통과했습니다. 설치 ZIP에는 SGB 코어·BIOS·게임·개인 세이브·진단 로그를 포함하지 않습니다.

[출처와 라이선스](https://github.com/hungrysanta-ksc/sd2snesHST/blob/master/THIRD-PARTY-NOTICES.md)
