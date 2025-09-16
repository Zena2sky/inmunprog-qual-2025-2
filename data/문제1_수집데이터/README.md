## 📂 문제1 수집 데이터

- **`kci_research_sample.csv`**  
  KCI API에서 **‘연구’** 키워드로 수집한 원본 데이터 (CSV 형식)

- **`kci_ai_sample.json`**  
  KCI API에서 **‘인공지능’** 키워드로 수집한 원본 데이터 (JSON 형식)

- **`kci_concat_with_category.csv`**  
  두 원본(연구 + 인공지능)을 **concat(세로 병합)** 하여 하나의 표로 만든 데이터.  
  각 레코드에는 `category` 컬럼이 추가되어, 연구/인공지능 구분이 가능합니다.

- **`kci_concat_with_meta.csv`**  
  `category` 정보에 더해, **추가 메타데이터(`domain`, `is_ai`)** 를 merge하여 확장한 버전.  
  → 이후 Kiwi 형태소 분석(문제 2-2)에서 연구/인공지능 텍스트 비교 분석에 활용됩니다.
