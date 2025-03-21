# 레시피 추천 시스템 (Recipe Recommendation System)

이 프로젝트는 **사용자의 취향**과 **재료 정보**를 바탕으로 적절한 레시피를 추천해주는 시스템입니다.  
프로젝트의 **주요 코드**는 `recipe_recommendation.ipynb`를 참고하시면 되고,  
**주제 선정 및 발표 내용**은 `presentation.pdf`에서 확인하실 수 있습니다.

---

## 목차
1. [프로젝트 개요](#프로젝트-개요)
2. [프로젝트 주요 기능](#프로젝트-주요-기능)
3. [폴더 구조](#폴더-구조)
4. [데이터 전처리 및 알고리즘 개요](#데이터-전처리-및-알고리즘-개요)
5. [사용 방법](#사용-방법)
6. [기술 스택 및 라이브러리](#기술-스택-및-라이브러리)
7. [프로젝트의 한계 및 개선 방향](#프로젝트의-한계-및-개선-방향)
8. [라이선스](#라이선스)
9. [문의](#문의)

---

## 프로젝트 개요
- **주제 선정**  
  - 온라인상의 방대한 레시피 중에서 **내가 가진 재료**와 **선호하는 음식**에 맞춰 손쉽게 찾을 수 있는 시스템의 필요성에서 출발하였습니다.

- **목표**  
  - 사용자가 **보유 중인 재료**와 **음식 선호도(매운 음식, 특정 재료 알레르기 등)**를 반영하여 레시피를 추천
  - 추천된 레시피에 **재료, 조리 시간 등 기본 정보**를 제공

- **발표 자료**  
  - 프로젝트 진행 과정과 자세한 발표 내용은 `presentation.pdf`를 참고해주세요.

---

## 프로젝트 주요 기능
1. **재료 입력**  
   - 사용자가 현재 보유하고 있는 재료를 입력하면, 해당 재료를 활용할 수 있는 레시피를 필터링합니다.

2. **선호도 반영**  
   - 매운 음식 선호 여부, 특정 알레르기(예: 견과류, 갑각류) 등 사용자의 기호를 추가로 반영하여 추천합니다.

3. **유사도 기반 레시피 추천**  
   - 레시피 간 유사도를 계산하여, 사용자가 입력한 키워드나 재료와 가장 유사도가 높은 레시피를 순위별로 제시합니다.

4. **추가 정보 제공**  
   - 추천된 레시피별로 필요한 재료, 조리 난이도, 소요 시간, 레시피 간단 요약 등을 함께 제공합니다.

---

## 폴더 구조

```bash
.
├── data
│   ├── raw_data.csv              # 원본 레시피/재료 데이터
│   ├── processed_data.csv        # 전처리된 데이터
├── recipe_recommendation.ipynb   # 프로젝트 주요 코드 (Jupyter Notebook)
├── presentation.pdf              # 발표 자료 (프로젝트 개요 및 결과)
├── README.md                     # 프로젝트 소개 문서 (현재 파일)
└── requirements.txt             # 프로젝트 환경설정에 필요한 라이브러리 목록
