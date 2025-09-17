# 데이터 제출용

본 레포는 2025-2학기 **인문지식처리와프로그래밍** 논문 제출 자격시험 데이터 제출용입니다.  
이론 답안 및 코드 파일은 포함하지 않고, **데이터 파일만** 포함합니다.

---

## 📂 폴더 구조

```data/
├── 문제1_수집데이터/
│   ├── kci_research_sample.csv        # KCI API에서 '연구' 키워드로 수집한 원본 데이터 (CSV)
│   ├── kci_ai_sample.json             # KCI API에서 '인공지능' 키워드로 수집한 원본 데이터 (JSON)
│   ├── kci_concat_with_category.csv   # 연구+인공지능 데이터 concat, category 컬럼 포함
│   └── kci_concat_with_meta.csv       # category + 추가 메타데이터(domain, is_ai) 병합본
│
└── 문제2_분석결과/
    ├── 1_preprocessing/               # 전처리 및 토큰화 결과
    │   ├── docs_from_processed.csv
    │   ├── tokens_from_processed.csv
    │   ├── processed_morphemes.pkl
    │   └── corpus_tokens.pkl
    │
    ├── 2_pos_analysis/                # 품사/빈도 분석
    │   ├── unigram_top50.csv
    │   ├── bigram_top50.csv
    │   ├── trigram_top50.csv
    │   ├── top_verbs_VV.csv
    │   ├── top_adjectives_VA.csv
    │   ├── pos_distribution.csv
    │   └── pos_distribution.png
    │
    ├── 3_keywords/                    # 키워드 및 시각화 결과
    │   ├── group_keywords_category.csv
    │   └── wordcloud_nouns_verbs.png
    │
    └── 4_hf_results/                  # HuggingFace 모델 적용 결과
        ├── hf_predictions_from_processed.csv
        ├── hf_predictions_from_processed.pkl
        └── label_keyword_top_from_processed_top20.csv   # 라벨별 상위 20개 키워드 (총 40개)


✍️ 본 리포지토리는 수업 과제 제출 및 재현 가능한 연구(Replicable Research)를 위해 코드, 데이터, 결과물을 함께 제공합니다.
