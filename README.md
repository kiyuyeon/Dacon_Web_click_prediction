### **README.md**  

# 웹 광고 클릭률 예측 AI 모델  

## **프로젝트 개요**  
이 프로젝트는 웹 광고 클릭률(Click-Through Rate, CTR)을 예측하기 위해 LightGBM(LGBM) 기반의 머신러닝 모델을 개발하는 데 중점을 둡니다.  
CTR 예측 모델은 디지털 마케팅과 온라인 광고 산업에서 고객의 행동을 분석하고 광고 효율성을 극대화하는 데 중요한 역할을 합니다.  

본 프로젝트에서는 웹 로그 데이터를 기반으로 CTR 예측 모델을 설계, 학습 및 평가했으며, 대용량 데이터 처리, 클래스 불균형, 고차원 데이터 등과 같은 실제 비즈니스 환경의 여러 문제를 해결하는 데 초점을 맞췄습니다.  

---

## **사용 기술 스택**  
- **Programming Language**: Python  
- **Machine Learning Framework**: LightGBM  
- **Data Handling**: Pandas, NumPy  
- **Evaluation Metrics**: Log Loss, AUC  
- **Visualization**: Matplotlib, Seaborn  

---

## **데이터 설명**  
- **Feature**: 웹 로그 데이터에서 수집된 광고 관련 피처  
- **Target**: `click` (1: 클릭, 0: 클릭하지 않음)  

데이터는 클래스 불균형을 가지며, 피처 중 일부는 높은 카디널리티(High Cardinality) 특성을 보입니다.  

---

## **모델 학습 및 평가**  
### **전처리 과정**  
1. 결측값 처리 및 이상치 제거  
2. 범주형 변수 인코딩 (Label Encoding, One-Hot Encoding 등)  

---

## **향후 개선 사항**  
1. **모델 성능 개선**  
   - 하이퍼파라미터 최적화 (Bayesian Optimization 등)  
   - 앙상블 기법 활용 (Stacking, Blending)  
2. **데이터 처리**  
   - 클래스 불균형을 해결하기 위한 샘플링 기법 추가  
   - Feature Selection을 통한 고차원 데이터 최적화  
3. **실시간 예측 시스템 구축**  
   - Flask 또는 FastAPI 기반의 예측 서비스 API 개발  
   - 배포 및 MLOps 파이프라인 구축  

---

