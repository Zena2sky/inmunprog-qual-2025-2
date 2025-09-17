### 문제2_분석결과

분석 코드는 Google Colab 노트북으로 별도 제출합니다.  
여기에는 **형태소 분석 및 텍스트 마이닝 응용 결과물**을 폴더별로 정리했습니다.

---

#### 📂 1_preprocessing (전처리 및 토큰화 결과)

- **`docs_from_processed.csv`**  
  전처리 완료된 문서 단위 데이터. 문장 단위/문서 단위의 분석에 활용.

- **`tokens_from_processed.csv`**  
  형태소 단위 토큰화 결과. 품사 태깅과 빈도 분석의 기본 데이터.

- **`processed_morphemes.pkl`**  
  형태소 분석 객체(pickle). 분석 재현성을 위해 저장.

- **`corpus_tokens.pkl`**  
  전체 코퍼스 토큰 정보(pickle). 대용량 데이터에서 빠른 재사용 가능.

---

#### 📂 2_pos_analysis (품사/빈도 분석)

- **`unigram_top50.csv` / `bigram_top50.csv` / `trigram_top50.csv`**  
  각 상위 50개 빈도표. 텍스트의 대표적 단어 조합을 보여줌.

- **`top_verbs_VV.csv`**  
  상위 동사(VV) 빈도. 연구 초록에서 동사 사용 경향 파악.

- **`top_adjectives_VA.csv`**  
  상위 형용사(VA) 빈도. 텍스트의 기술적/서술적 성격 해석에 활용.

- **`pos_distribution.csv` / `pos_distribution.png`**  
  품사별 분포 통계 및 시각화. 전체 텍스트에서 어떤 품사가 두드러지는지 확인 가능.

---

#### 📂 3_keywords (키워드 및 시각화 결과)

- **`group_keywords_category.csv`**  
  주요 키워드를 그룹별(연구/인공지능)로 집계. 카테고리별 차이 비교.

- **`wordcloud_nouns_verbs.png`**  
  명사·동사 워드클라우드. 직관적으로 핵심 단어를 시각화하여 표현.

---

#### 📂 4_hf_results (HuggingFace 모델 적용 결과)

- **`hf_predictions_from_processed.csv`**  
  HuggingFace 모델의 전체 예측 결과 (CSV)

- **`hf_predictions_from_processed.pkl`**  
  동일한 예측 결과를 저장한 pickle 버전 (재현성·재사용 목적)

- **`label_keyword_top_from_processed_top20.csv`**  
  라벨(인공지능/일반)별 상위 20개 키워드 (총 40개) 집계 결과

