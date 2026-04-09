# 2025 DONGWON x KAIST AI Competition 대상
: **Statistical Modeling + LLM Simulation 기반 4STAGE 수요 예측 전략**

본 프로젝트는 기존의 시장 조사를 통한 수요 예측의 한계를 보완하기 위해 통계 분석과 LLM Simulation을 결합한 Hybrid 수요 예측 전략을 설계하고, 이를 통해 동원 그룹 신제품 15종의 월별 판매량을 예측하는 것을 목표로 합니다.

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


![Dongwon PPT](https://github.com/olchan/DONGWONxKAIST-AI-Competition/blob/main/Dongwon%20PPT.png?raw=true)

![Dongwon PPT](https://github.com/olchan/DONGWONxKAIST-AI-Competition/blob/main/Dongwon%20PPT%20(1).png?raw=true)

![Dongwon PPT](https://github.com/olchan/DONGWONxKAIST-AI-Competition/blob/main/Dongwon%20PPT%20(2).png?raw=true)

![Dongwon PPT](https://github.com/olchan/DONGWONxKAIST-AI-Competition/blob/main/Dongwon%20PPT%20(3).png?raw=true)

![Dongwon PPT](https://github.com/olchan/DONGWONxKAIST-AI-Competition/blob/main/Dongwon%20PPT%20(4).png?raw=true)

![Dongwon PPT](https://github.com/olchan/DONGWONxKAIST-AI-Competition/blob/main/Dongwon%20PPT%20(5).png?raw=true)

![Dongwon PPT](https://github.com/olchan/DONGWONxKAIST-AI-Competition/blob/main/Dongwon%20PPT%20(6).png?raw=true)
