# MrBoBot

MrBoBot은 디스코드 서버에서 음악을 재생하고 관리할 수 있는 봇입니다. 음악 재생, 대기열 관리, 버튼 컨트롤, 그리고 다양한 명령어를 제공합니다.

## 주요 기능
- **음악 재생 및 제어**: YouTube 링크 또는 검색어를 통해 음악을 재생할 수 있습니다.
- **대기열 관리**: 음악 대기열 출력, 특정 곡 삭제 기능 지원.
- **버튼 컨트롤**: 재생, 일시정지, 재개, 스킵, 정지 버튼 제공.
- **명령어 도움말**: 사용 가능한 모든 명령어를 한눈에 확인 가능.

## 사용법
### 명령어 목록
- `!play <검색어>`: 유튜브에서 검색어로 음악을 찾아 재생하거나 대기열에 추가합니다.
- `!playlist`: 현재 대기열에 있는 음악 목록을 출력합니다.
- `!remove <번호>`: 대기열에서 특정 번호에 해당하는 음악을 삭제합니다.
- `!stop`: 현재 재생 중인 음악을 정지합니다.
- `!pause`: 현재 재생 중인 음악을 일시 정지합니다.
- `!resume`: 일시 정지된 음악을 재개합니다.
- `!skip`: 현재 재생 중인 음악을 스킵하고 다음 음악을 재생합니다.
- `!help`: 모든 명령어와 사용법을 출력합니다.

### 버튼 컨트롤
음악이 재생될 때 디스코드 메시지에 나타나는 버튼을 통해 음악을 쉽게 제어할 수 있습니다:
- **Stop**: 음악 정지
- **Pause**: 음악 일시 정지
- **Resume**: 음악 재개
- **Skip**: 현재 곡 스킵

## 파일 구조
```
MrBoBot/
├── bot.py # 봇의 메인 실행 파일
├── config.py # 환경 변수 로드 및 봇 설정
├── cogs/ # Cog(명령어) 모듈 폴더
│ ├── general.py # 일반 명령어 정의
│ └── music_cog.py # 음악 관련 명령어 정의
├── utils/ # 유틸리티 함수 폴더
│ └── youtube.py # 유튜브 검색/다운로드 함수
├── requirements.txt # Python 패키지 목록
├── run_bot.bat # Windows용 실행 스크립트
└── README.md # 프로젝트 설명 파일
```

## 설치 및 실행 방법
1. 이 저장소를 클론합니다:
   ```bash
   git clone https://github.com/yourusername/MrBoBot.git
   ```
2. 프로젝트 폴더로 이동합니다:
   ```bash
   cd MrBoBot
   ```
3. Python 가상 환경을 생성하고 활성화합니다:
   ```bash
   python -m venv venv
   source venv/bin/activate  # Windows는 venv\Scripts\activate
   ```
4. 필요한 패키지를 설치합니다:
   ```bash
   pip install -r requirements.txt
   ```
5. `.env` 파일을 생성하고 디스코드 봇 토큰을 추가합니다:
   ```
   DISCORD_BOT_TOKEN=your_discord_bot_token
   ```
6. 봇을 실행합니다:
   ```bash
   python bot.py
   ```

## 요구사항
- Python 3.8 이상
- 디스코드 봇 토큰

## 주의사항
- `.env` 파일에 저장된 봇 토큰은 절대 공개 저장소에 업로드하지 마세요.
- 음악 재생은 YouTube 링크를 기반으로 하며, 인터넷 연결이 필요합니다.

## 기여하기
이 프로젝트에 기여하고 싶다면 언제든 Pull Request를 보내주세요!

## 라이선스
이 프로젝트는 MIT 라이선스 하에 배포됩니다. 자세한 내용은 LICENSE 파일을 참조하세요.

