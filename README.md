# DScover_24-2_MainProject_TeamA

### 프로젝트 주제
청년 농부를 위한 스마트 노지 통합 서비스
-작물별 최적의 스마트 노지 입지 분석을 기반으로

### 프로젝트 개요
농업 인구의 고령화 문제를 해결하기 위해 귀농을 고려하는 예비 청년 농부를 대상으로 작물별 최적의 입지 추천 및 컨설팅 리포트 제공, 유통망 매칭 서비스를 포함한 통합 웹 서비스를 제공하고자 한다.

### 데이터 수집
crop_df: 선정한 11개 작물의 생육기간, 적정기온, 적정 월 평균 강수량, 적정 일조량 데이터 수집  
region_df: 기상청 기후+지점 데이터, 불투수율, 행정동별 농업 면적 데이터 수집

### 분석방법
> 1. 스마트 노지 입지 분석
  region_df 내에서 비슷한 조건을 가진 행정동 클러스터링
  crop_df와의 유클리드 거리를 계산하여 행정동 군집과 최적의 작물 매칭
  
> 2. 청년 농부 컨설팅 리포트
  GPT api를 활용한 컨설팅 리포트 출력
  예상 수익 및 경영비, 브랜드 스토리, 스마트 노지 경영 전략 포함

> 3. 유통망 매칭
  전국 유통센터, 도매시장, 공판장 데이터 수집
  하버사인 지표를 활용한 경계범위 내 유통망 추천

> 4. 웹사이트 구축
  streamlit 라이브러리를 활용한 웹사이트 구축 및 배포 
