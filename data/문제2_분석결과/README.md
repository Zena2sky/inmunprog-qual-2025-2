# 🗂️ 문제2 분석 결과

이 폴더에는 문제1에서 수집·가공한 데이터를 바탕으로 수행한 형태소 분석 및 응용 분석 결과가 포함되어 있습니다.  
분석 코드는 별도로 Google Colab 노트북으로 제출합니다.

---

## 1. 전처리 및 토큰화 결과
- **docs_from_processed.csv** : 전처리 완료된 문서 단위 데이터
- **tokens_from_processed.csv** : 형태소 단위 토큰화 결과
- **processed_morphemes.pkl** : 형태소 분석 객체(pickle 저장)
- **corpus_tokens.pkl** : 전체 코퍼스 토큰 정보(pickle 저장)

## 2. 품사/빈도 분석
- **unigram_top50.csv / bigram_top50.csv / trigram_top50.csv** : 단일어/이중어/삼중어 상위 50개 빈도표
- **top_verbs_VV.csv** : 상위 동사(VV) 빈도
- **top_adjectives_VA.csv** : 상위 형용사(VA) 빈도
- **pos_distribution.csv / pos_distribution.png** : 품사별 분포 통계 및 시각화

## 3. 키워드 및 시각화 결과
- **group_keywords_category.csv** : 주요 키워드 그룹별 집계
- **wordcloud_nouns_verbs.png** : 명사·동사 워드클라우드

## 4. HuggingFace 모델 적용 결과
- **hf_predictions_from_processed.csv / .pkl** : HuggingFace 모델 예측 결과 (CSV 및 pickle)
- **label_keyword_top_from_processed_top20.csv** : 예측 라벨 기준 상위 20개 키워드

---

📌 정리:
- CSV는 수치·표 데이터  
- PNG는 시각화 이미지  
- PKL은 중간 객체(재현 가능성 보장용)

