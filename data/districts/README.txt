구역 DB 사용법
==============

- 00.json ~ 72.json 중 원하는 파일 하나만 수정하면 됩니다.
- 공통 플레이스홀더는 ../defaults.json에서 관리합니다.
- 파일의 id는 파일명과 같게 유지하세요. 예: 04.json -> "id": 4
- 비워 둔 필드는 공통 플레이스홀더 또는 화면의 자동 위치값으로 처리됩니다.

기본 필드
---------
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
