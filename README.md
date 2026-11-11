# CMC (Comms Material Clearance) — 통신자재 수입허가 서류 작성

이라크 CMC(통신미디어위원회) 통신자재 Type Approval 서류를 만드는 웹 도구입니다.

## 만들어지는 서류 (ZIP)
1. NIC 공문 (영문 + 아랍어, ALE 면세신청 공문 양식)
2. CMC APPLICATION FOR TYPE APPROVAL (모델별 또는 합본)
3. 시리얼 번호 목록 (엑셀)

## 사용 순서
1. 패킹리스트/CIPL 엑셀을 올립니다 → 모델·수량·HS·시리얼 자동 입력
2. 시험성적서·원산지증명(COO)·사양서 PDF/사진을 올립니다 → 제조사·원산지·시험정보·인증규격 자동 입력 (노란 칸)
3. 노란 칸과 빈 칸을 확인·수정합니다
4. 서류 만들기 → ZIP 다운로드 → Word에서 최종 확인 후 출력

## 참고
- 스캔본(이미지) 인식은 GitHub Pages 주소로 열었을 때만 됩니다. 파일을 더블클릭해서 열면 엑셀·글자 PDF만 읽습니다.
- 모든 처리는 브라우저 안에서만 이뤄지고 파일은 어디에도 전송되지 않습니다.
- 고정 정보는 브라우저에 저장됩니다. "설정 내보내기/불러오기"로 다른 PC와 공유하세요.

## 신청서 항목별 자동 입력 범위
| 신청서 항목 | 자료 | 결과 |
|---|---|---|
| Model · 수량 · HS · Brief Description | 패킹리스트(PL) | 자동 |
| Equipment Name · Type of Equipment | PL 품목 설명 | 자동 추정 |
| Manufacturer · Country · Address | 원산지증명(COO) | 자동 (COO 없으면 빈칸) |
| Year of Manufacturing | 시험성적서 일자 | 자동 |
| Software Version | 시험성적서 펌웨어 | 자동 (스캔본 숫자 확인 필요) |
| Test report · Test Name · Test No. · Date | 시험성적서 | 자동 |
| Test standard | 사양서 인증 항목 | 자동 (모델별) |
| Test Laboratory | 자료 없음 | 제조사명 자동 입력 → 확인 필요 |
| Hardware Version | 자료 없음 | 기본값 N/A → 수기 확인 |
