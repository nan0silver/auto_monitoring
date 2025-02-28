### 📌 **도지코인 트렌드 대시보드**  

이 프로젝트는 **도지코인(Dogecoin) 뉴스 및 트렌드를 분석하고 GitHub Pages로 자동 배포하는 대시보드**입니다.  
매일 최신 뉴스 데이터를 가져와 OpenAI LLM을 활용하여 분석하며, 한국 시간 **오전 8시(KST)** 에 자동 업데이트됩니다.

🔗 **사이트 바로가기:** [GitHub Pages에서 보기](https://nan0silver.github.io/auto_monitoring/)

---

## 🚀 **기능**
✅ 최신 도지코인 뉴스 자동 수집 및 LLM 분석  
✅ 감성 분석 및 미래 트렌드 예측 제공  
✅ **Chart.js**를 이용한 가격 변동 그래프 표시  
✅ **GitHub Actions**를 활용한 자동 업데이트 (매일 오전 8시 KST)  

```mermaid
flowchart LR
    A[GitHub Actions 실행] -->|스케줄 또는 수동 트리거| B[Java 프로그램 실행]
    B --> C[네이버 API로 키워드 뉴스 검색]
    C --> D[뉴스 데이터 추출]
    D --> E[GPT-4 API로 뉴스 분석]
    B --> F[네이버 API로 관련 이미지 검색]
    F --> G[이미지 다운로드]
    E --> H[Markdown 파일 생성]
    G --> H
    H --> I[GitHub에 결과물 커밋]
    I --> J[Jekyll로 사이트 빌드]
    J --> K[GitHub Pages로 배포]
```

---


## 📊 **사용 기술**
- **Backend:** Java (HTTP 요청, JSON 파싱)
- **Data Analysis:** OpenAI LLM (gpt-4)
- **Visualization:** Chart.js
- **Deployment:** GitHub Pages, GitHub Actions  

---
