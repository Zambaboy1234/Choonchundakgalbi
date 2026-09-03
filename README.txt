EMBER MAP PROTOTYPE // DATA LAYOUT
===================================

구역 데이터는 한 파일에 몰아넣지 않고 구역별로 분리되어 있습니다.

data/defaults.json
- 모든 구역에 적용되는 플레이스홀더 기본값

data/districts/00.json ~ 72.json
- 해당 구역의 이름, 인용구, 설명, 지도부, 위치, 대표 산업, 노트 등을 수정하는 파일
- 한 구역을 수정할 때 해당 번호의 파일 하나만 편집하면 됩니다.

각 파일의 기본 필드
-------------------
{
  "id": 4,
  "name": "구역 이름",
  "logo": "assets/logos/district-04.png",
  "quote": "구역 대표 인용구",
  "description": "구역 본 설명문",
  "leadership": "지도부 또는 운영 주체",
  "location": "북부 / 동부 / 남부 / 서부",
  "industry": "대표 산업",
  "note": "소장 또는 대원이 남긴 짧은 기록",
  "noteAuthor": "인용자"
}

정적 배포
---------
index.html은 위 JSON 파일들을 fetch로 읽습니다. GitHub Pages처럼 HTTP로
제공되는 환경에서는 그대로 작동합니다. index.html을 파일 탐색기에서
직접 여는 file:// 방식은 브라우저 보안 정책 때문에 JSON을 읽지 못할 수
있으므로, 로컬 테스트 시 간단한 정적 서버를 사용하세요.
