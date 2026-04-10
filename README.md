# 🥇 2025 DONGWON x KAIST AI Competition 대상
: **Statistical Modeling + LLM Simulation 기반 4STAGE 수요 예측 전략**

<img width="400" alt="dongwon" src="https://github.com/user-attachments/assets/0552e49d-d64a-4d9e-b902-56cd575b67ac" />

## 🎥 발표 영상
<div>
  <a href="https://www.youtube.com/live/dk7gubnleaI?si=VocQFSGNO05iLjUS&t=14081">
    <img width="400" alt="image" src="https://github.com/user-attachments/assets/49ecea93-f83a-43cd-8a6a-e6c3a46ecaa1" />
  </a>
  <br/>
</div> 

<div>
  
> 본 프로젝트는 기존의 시장 조사를 통한 수요 예측의 한계를 보완하기 위해 통계 분석과 LLM Simulation을 결합한 Hybrid 수요 예측 전략을 설계하고, 이를 통해 동원 그룹 신제품 15종의 월별 판매량을 예측하는 것을 목표로 합니다.

> 📰 [기사 바로 보기](https://m.sedaily.com/article/14125622)
</div> 

## Key Idea
LLM은 상대적 선호 비교에는 강하지만, 절대적인 수요 규모(Scale) 추정에는 한계가 있기에,
1. 통계 기반 분석을 통한 시장 규모 계산
2. 제품 특징을 반영한 LLM Persona 생성
3. LLM Simulation 기반 선택 확률 추정
4. Trend 및 출시일 정보를 반영

## 📊 Result

- 15개 신제품 수요 예측 수행
- sMAPE: **0.26**
- Benchmark (E2open, Forecasting and Inventory Benchmark Study, 2019): **0.48**


## 🤖 LLM Setup

### Persona Generation
- Model: EXAONE 4.0 32B
- Platform: FriendlyAI
- Purpose: 인구 분포 기반 소비자 페르소나 생성

### Simulation (Inference)
- Model: EXAONE 3.5 7.8B (AWQ Quantized)
- Hardware: NVIDIA RTX 3070 (Local)
- Purpose: 반복 시뮬레이션을 통한 선택 확률 분포 생성

## 📚 References

- Brand, J., Israeli, A., & Ngwe, D. (2023), *Using LLMs for Market Research*. Harvard Business School Working Paper No. 23-062.
- LLM이 반복적인 응답 생성을 통해 "응답 분포"를 형성하며, 실제 소비자 설문과 유사한 WTP 추정이 가능함을 실증적으로 확인
 👉 기존 연구에서 제시된 한계(LLM의 bias 및 variability)를 고려하여, 본 프로젝트에서는 LLM을 "상대적 선호 추정"에만 사용하고 절대 수요(Scale)는 통계 분석 방식으로 분리하여 전체 예측값을 도출하였다.
- https://www.hbs.edu/ris/Publication%20Files/23-062_6bfe7a5b-3ed9-4afd-a4c1-c91b60dd82e5.pdf  




<img width="1920" height="1080" alt="Dongwon PPT" src="https://github.com/user-attachments/assets/171c34c2-5b25-4a75-a77a-ed5099cc33ae" />
<img width="1920" height="1080" alt="Dongwon PPT (1)" src="https://github.com/user-attachments/assets/577fd3aa-efea-463f-b16a-2fd28ea7959c" />
<img width="1920" height="1080" alt="Dongwon PPT (2)" src="https://github.com/user-attachments/assets/4a37cf79-9045-4068-8dd4-f1f22da5d603" />
<img width="1920" height="1080" alt="Dongwon PPT (3)" src="https://github.com/user-attachments/assets/c7f2b695-ded5-4bf5-b0cc-f394241ca7b8" />
<img width="1920" height="1080" alt="Dongwon PPT (4)" src="https://github.com/user-attachments/assets/2143b477-69bf-4ff9-b76f-8838bc185225" />
<img width="1920" height="1080" alt="Dongwon PPT (5)" src="https://github.com/user-attachments/assets/62a8f35b-95c4-450a-97a5-8a60f5bfe2c8" />
<img width="1920" height="1080" alt="Dongwon PPT (6)" src="https://github.com/user-attachments/assets/0d3eb6dd-7db8-450e-90f2-356176a9b26c" />
<img width="1920" height="1080" alt="Dongwon PPT (7)" src="https://github.com/user-attachments/assets/db0891b8-3215-41b8-975f-4f599364f12d" />
