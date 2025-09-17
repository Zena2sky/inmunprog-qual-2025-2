#### 📂 4_hf_results (HuggingFace 모델 적용 결과)

이 폴더는 **문제 2-2 실습 (고급 응용 분석 – HuggingFace 분류/예측)** 의 핵심 산출물입니다.  

- **`hf_predictions_from_processed.csv`**  
  모든 문서에 대해 HuggingFace 모델이 예측한 라벨 결과 (CSV 형식).  
  → 전체 데이터셋에 대한 **원시 예측 결과**이며, 후속 분석의 기반 데이터.

- **`hf_predictions_from_processed.pkl`**  
  동일한 예측 결과를 Python 객체(pickle)로 저장한 버전.  
  → CSV보다 로딩이 빠르고, 재현성 보장. 후속 분석이나 추가 실험 시 재사용 가능.

- **`label_keyword_top_from_processed_top20.csv`**  
  예측된 라벨(예: **인공지능 vs 일반**)별로 자주 등장한 키워드를 집계하고,  
  각 라벨별 상위 20개씩 추출한 결과 → **총 40개 키워드**.  
  → 라벨별 “대표 키워드”를 보여주는 **하이라이트 산출물**로,  
  단순 분류 정확도를 넘어 **라벨별 텍스트 특성을 해석**할 수 있는 단서를 제공합니다.
