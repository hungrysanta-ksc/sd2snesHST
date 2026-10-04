# sd2snesHST 0.9.0

HungrySanTa의 FXPAK Pro 추가 코어 프로젝트 첫 릴리스입니다. **검증된 GBC C44와 동일한 실행 파일**을 사용합니다.

## 설치
FXPAK Pro / Mk.III의 정상 설치된 공식 sd2snes 1.11.2 계열 위에 적용합니다. 기존 SD를 백업하고 업데이트 ZIP의 파일을 합쳐 복사하세요. 동봉 RTC 시차는 한국/일본용 +540이며 기존 사용자 설정이 맞으면 유지합니다.

[사용 가이드](https://github.com/hungrysanta-ksc/sd2snesHST/blob/master/docs/USER-GUIDE.ko.md) · [호환성](https://github.com/hungrysanta-ksc/sd2snesHST/blob/master/docs/COMPATIBILITY.ko.md)

## 파일 선택
- **sd2snesHST-v0.9.0-update.zip**: 설치용 업데이트와 사용 가이드.
- **sd2snesHST-v0.9.0-source.zip**: 고정 C44 구현 소스·빌드 지침.
- **sd2snesHST-v0.9.0-manifest.json**: 대상 보드·소스·실행 파일·ZIP의 대응 관계.
- **SHA256SUMS.txt**: 위 3개 파일의 SHA256.

GitHub 자동 생성 Source code ZIP은 사용자 안내 저장소의 사본이며 펌웨어 소스 묶음이 아닙니다.

## 기능과 범위
.egbc GB/GBC 코어, SRAM·자동 기록, MBC3 RTC, 강제 저장 4슬롯, R 버튼 약 3배 빨리감기, 소리 설정, 게임 리셋을 제공합니다. load/cap/state 진단 로그는 생성하지 않습니다.

기존 .gb/.gbc는 SGB 경로를 사용합니다. SGB 코어·BIOS·게임·개인 세이브는 포함하지 않습니다. NES·PCE는 이번 버전에 포함하지 않습니다.

## 초안 검토
아직 공개 릴리스가 아닙니다. 설치 파일 해시와 소스 대응은 검증했으며, 공개 전에는 출처·배포 고지의 미결 범위를 정리하고 README의 준비 중 안내를 전환합니다.
