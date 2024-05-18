# GSA-lol-esports-manual

[![2024 LCG Grand Final](http://img.youtube.com/vi/fPvCNqmRiMA/0.jpg)](https://youtube.com/live/fPvCNqmRiMA?feature=share)

위의 예시 영상은 2024년에 진행한 대회의 송출 영상입니다.

## 1. 준비물

### 1.1 송출용 컴퓨터

송출용 컴퓨터는 관전용 컴퓨터와 리소스 서버용 컴퓨터의 화면을 받아 유튜브 송출을 담당하는 컴퓨터입니다.

- OBS
- (관전용 컴퓨터와 무선 연결시) NDI Plugin

### 1.2 관전용 컴퓨터

관전용 컴퓨터는 인게임을 관전하며, 밴픽 화면을 만들어 송출용 컴퓨터로 화면을 송출하는 컴퓨터입니다.

- League of Legends
- VPN (학교 와이파이에서 접속을 위함. 여러가지 프로그램이 있으나 Cloudflare Warp 추천)
- (송출용 컴퓨터와 무선 연결시) NDI Plugin
- OBS
- [lol-pick-ban-ui](https://github.com/RCVolus/lol-pick-ban-ui) 세팅

> **주의사항**
> 
> 2024년 당시 대회를 준비할 때는 [league-prod-toolkit](https://github.com/RCVolus/league-prod-toolkit)에 문제([해당이슈](https://github.com/RCVolus/league-prod-toolkit/issues/668))가 있었기에 [lol-pick-ban-ui](https://github.com/RCVolus/lol-pick-ban-ui)를 사용했습니다.
> 만약 대회를 준비할 때, [league-prod-toolkit](https://github.com/RCVolus/league-prod-toolkit)에 나와있는 방법대로 설치를 진행하여 문제가 생기지 않는다면 [league-prod-toolkit](https://github.com/RCVolus/league-prod-toolkit)를 사용하는 것이 더 좋습니다. 
> 
> 밴픽화면만 있는 [lol-pick-ban-ui](https://github.com/RCVolus/lol-pick-ban-ui)와 달리 [league-prod-toolkit](https://github.com/RCVolus/league-prod-toolkit)는 인게임 레이아웃, 게임이 끝난 뒤 스탯 화면등이 제공됩니다.
> 라이엇 api는 키를 발급받아서 사용하시면 됩니다.

> **주의사항**
> 
> 위의 예시 영상에서 밴픽과 인게임 화면에서 팀 이름이 표시되는 화면은 [league-prod-toolkit](https://github.com/RCVolus/league-prod-toolkit)에서 module-teams 기능만 설치하여 사용한 결과입니다.

### 1.3 리소스 서버용 컴퓨터

리소스 서버는 송출용 컴퓨터의 브라우저 리소스(카운트다운 화면 등)을 호스팅하는 컴퓨터입니다.

- Node.js
- Ngrok(localhost를 외부에서 접속할 수 있게 해주는 프로그램)
- 이 repository의 코드들