# Proposal AI

> KT에서 제안서를 작성할때 입찰전략을 수립해주는 LLM 기반 PoC 서비스

[![Python 3.12](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)](https://www.python.org/downloads/release/python-3120/)
[![HuggingFace](https://img.shields.io/badge/HuggingFace-Meta-Llama-3-8B-yellow?logo=huggingface&logoColor=white)](https://https://huggingface.co/meta-llama/Meta-Llama-3-8B)


---

## 1. 프로젝트 개요
**proposal AI**는 KT에서 AICC 제안서를 작성할때 입찰전략을 수립해주는 LLM 기반의 PoC 서비스입니다. 나라장터 최근 7년간의 입찰사업의 입찰가격, 평가점수, 세부분야 및 뉴스 동향을 기반으로 경쟁사와의 경쟁우의 및 전략을 파악하고 수립해주는 서비스를 제공합니다. 본 프로젝트는 KT AICT Future TF 2차 프로젝트

**주요 기능:**
- **경쟁사 우위 비교:** 다양한 정보들을 기반하여 입찰하고자 하는 사업의 경쟁사의 최근 뉴스 및 주요 기술을 분석하여, 경쟁사와의 경쟁우의를 비교해줍니다.
- **입찰 가격 추천:** 최근 나라장터 내 프로젝트 종류별 입찰가격 추이를 기반하여, 입찰하고자 하는 사업의 입찰 참여 가격을 제안해줍니다.  
- **입찰 전략 수립:** 최근 뉴스 동향 및 경쟁사 주요 기술등을 파악하여, 입찰하고자 하는 사업의 입찰 참여 전략을 제안해줍니다.

**처리 흐름:**
- **모델 사전학습:** pre-training domain knowledge
- **모델 파인튜닝:** fine-tunning LLM Model
- **프롬프트 엔지니어링:** prompt enginnering with unit of proposal assistant services
- **UI 구성:** deploy on website with Gradio


---


## 2. 기술 스택
> Hugging Face 기반의 LLM 모델을 활용하였습니다.

| 분류 | 구성 요소 |
| --- | --- |
| Language | Python 3.12 |
| AI Model | Llama |


---


## 3. 실행 방법
> Google Colab 기반으로 실행 가능합니다. 

- Google Colab: [https://colab.research.google.com/](https://colab.research.google.com/)


---


## 4. 주요 모듈 구성 및 기능

```
proposal_ai/
├── README.md                       # 서비스 개요
├── proposal_ai_demo_video.mp4      # 데모 비디오
├── proposal_ai_ppt.pptx            # 발표자료
├── proposal_ai_source_code.ipynb   # 메인 소스코드
└── dataset/                        # 주요 데이터셋
    ├── aicc_dataset.csv
    └── company_article.csv
```


