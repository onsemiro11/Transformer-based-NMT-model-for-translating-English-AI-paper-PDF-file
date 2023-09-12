# Transformer-based-NMT-model-for-translating-English-AI-paper-PDF-file

# 개발 배경

시중에 네이버 파파고, 구글 번역기 등 여러 번역기가 나와 있습니다. 하지만 특정 도메인 지식을 반영하여 번역하지 못한다는 단점을 파악하였습니다. 예를 들어, 이상 탐지 알고리즘 논문에 contamination을 '오염'이라고 번역합니다. 하지만 도메인 지식에 따르면 '데이터의 불순도'로 의역할 수 있습니다. 이러한 점을 반영하여 (1) 영문 인공지능 논문을 한국어로 번역하여 학생들이 더욱 편하게 읽을 수 있도록 하고자 주제를 선정하였습니다. 그리고 논문의 문장을 하나하나 스크롤 하여 번역기에 입력하는게 불편하여 PDF의 텍스트 또한 편리하게 (2)PDF를 입력하면 이미지로 변환하고 변환된 이미지의 텍스트를 인식하여 한영 번역을 해주는 기계번역 모델(NMT)를 구축하는 것을 목표로 프로젝트를 진행했습니다.

# 프로젝트 과정

1. 수집한 데이터를 학습 데이터로 사용할 수 있도록 준비
2. Transformer를 통해 기술과학 논문 영한 번역 데이터와 일상 구어체 데이터를 통해 학습
3. OCR(Optical Character Recognition) 기술로 PDF에서 텍스트를 추출
4. 츠츨한 텍스트를 transformer 모델을 통해 추론(번역)

# Project Overview

![image](https://github.com/onsemiro11/Transformer-based-NMT-model-for-translating-English-AI-paper-PDF-file/assets/49609175/724dc515-e076-4cd0-adc4-84c3fb5ac517)

# 수집한 데이터

- AI hub "기술과학 분야 한-영 번역 병렬 말뭉치 데이터"

인공지능, 빅데이터, IT 분야의 데이터만 가져와서 20만개 말뭉치를 활용했다.
