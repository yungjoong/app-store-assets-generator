# App Store Assets Generator (v3.1)

HTML/JS 기반의 앱 스토어 마케팅 자산(스크린샷, 피처 그래픽) 자동 생성 도구입니다.

## 📁 폴더 구조
- MARKETING_DASHBOARD.html: 메인 대시보드 (자산 생성 및 다운로드)
- templates/
  - marketing_template.html: 스크린샷 템플릿
  - google_play_feature_graphic.html: 구글 플레이 피처 그래픽 템플릿

## 🚀 사용법 (프로젝트 적용 방법)
1. 이 저장소의 모든 파일을 프로젝트 루트(marketing-tool/ 등)에 복사하거나 git submodule로 추가합니다.
2. 터미널에서 로컬 서버를 실행합니다: npx serve . (이미지가 CORS 문제 없이 로드되려면 서버 실행이 필수입니다.)
3. 브라우저에서 http://localhost:3000/MARKETING_DASHBOARD.html에 접속합니다.

## ⚙️ 설정 방법
MARKETING_DASHBOARD.html 내의 languages 배열을 프로젝트에 맞게 수정하여 사용하세요:
- code: 언어 코드 (예: ko, en)
- name: 표시 언어 이름
- title: 앱 제목
- screens: 01~05번까지의 스크린샷 상단 문구 리스트

## 📸 스크린샷 파일 규칙
store-assets/screenshots/{device_id}/{device_id}_{lang}_{num}_{suffix}.png 규칙을 따릅니다.
(예: phone/phone_ko_01_main.png)
파일이 없는 경우 자동으로 영문(en) 버전으로 대체(fallback)됩니다.

---
💡 Tip: MARKETING_DASHBOARD.html 최하단의 "통합 패키지 다운로드"를 사용하여 모든 언어의 자산을 한 번에 관리하세요.
