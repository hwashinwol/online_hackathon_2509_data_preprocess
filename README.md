# 🛠️ Data Preprocessing & Embedding Pipeline
> AI Hub '정신건강 상담 데이터' 전처리 및 벡터 임베딩 파이프라인 저장소

## 📂 Project Overview
본 프로젝트는 **우울/불안 감지 AI 챗봇** 개발 과정에서 대용량 텍스트 데이터의 로딩 속도를 최적화하기 위해 구축된 전처리 모듈입니다.

## 🔑 Key Features
1. **Symptom-based Partitioning (증상별 데이터 분할)**
   - 전체 데이터를 4가지 카테고리로 분리하여 관리 효율성 증대
   - `dep` (Depression, 우울증)
   - `anx` (Anxiety, 불안장애)
   - `add` (Addiction, 중독)
   - `nor` (Normal, 일반/기타)

2. **Embedding Serialization (임베딩 직렬화)**
   - 매 실행 시 발생하는 임베딩 연산 비용(Time Cost)을 절감하기 위해 `Pickle(.pkl)` 형태로 벡터값 저장
   - 40만 토큰 이상의 텍스트 데이터를 사전에 벡터화하여 검색 속도 개선 시도

## 🛠️ Tech Stack
- **Python, Pandas** (데이터 정제)
- **Pickle** (객체 직렬화)
- **Sentence-Transformers** (벡터 임베딩)

***모델링 코드를 포함하고 있지 않음***
