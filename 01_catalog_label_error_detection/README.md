# Catalog Label Error Detection

쿠팡 카탈로그의 **상품명 · 카테고리 · 옵션** 간 불일치 정보를 자동으로 탐지하는 모델을 구축한 프로젝트입니다.

## 1. Goal
- 상품 정보의 라벨 오류를 자동으로 탐지하여 데이터 품질을 향상
- 불일치로 인한 반품, CS 증가 문제를 예방

## 2. Data
- 직접 생성한 샘플 상품 데이터  
- 컬럼: product_name, category_name, option, brand, price 등

## 3. Methods
- 형태소 분석 (Mecab)
- TF-IDF / Word2Vec 임베딩
- Logistic Regression / Random Forest
- Precision, Recall, F1-score 평가

## 4. Results
- F1-score: 0.84  
- 특정 카테고리(의류)에서 성능 우수  
- 잘못된 사이즈/성별 태그 오류 탐지 가능

## 5. Future Work
- 실제 쿠팡 카탈로그 속성 체계 반영  
- BERT 기반 다중 레이블 모델 확장
