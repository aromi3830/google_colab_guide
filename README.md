# google_colab_guide

# 🚀 구글 코랩(Colab) 완전 가이드

구글 코랩(Google Colaboratory)은 클라우드 기반의 파이썬 실행 환경으로, 머신러닝, 데이터 분석, 교육용 프로젝트 등에 매우 유용합니다. 이 문서는 **코랩의 기본부터 고급 기능까지** 체계적으로 설명합니다.

---

## 📚 목차

| 구분 | 내용 |
|------|------|
| 1. [Colab 소개](#1-colab-소개) | Colab의 개념과 특징 |
| 2. [기본 사용법](#2-기본-사용법) | 노트북 생성, 셀 실행 등 |
| 3. [파일 입출력](#3-파일-입출력) | Google Drive 연동, 파일 업/다운로드 |
| 4. [코랩 환경 제어](#4-코랩-환경-제어) | 런타임 관리, GPU 설정 등 |
| 5. [고급 기능](#5-고급-기능) | 마크다운, 폼(Form), 매직 명령어 |
| 6. [자주 발생하는 오류 & 해결법](#6-자주-발생하는-오류--해결법) | 실전 팁 |
| 7. [자주 묻는 질문(FAQ)](#7-자주-묻는-질문faq) | 사용자 질문 정리 |

---

## 1. Colab 소개

| 항목 | 설명 |
|------|------|
| 이름 | Google Colaboratory |
| 개발 | Google Research |
| 장점 | 무료 GPU 사용 가능, 설치 필요 없음, 구글 드라이브와 연동 |
| 용도 | 데이터 과학, 딥러닝 실험, 교육 등 |

> 💡 Colab은 Jupyter Notebook을 기반으로 동작합니다.

---

## 2. 기본 사용법

### 📄 노트북 생성

1. [https://colab.research.google.com](https://colab.research.google.com) 접속
2. `새 노트북` 클릭

### ▶️ 셀 실행

- 코드 셀: 파이썬 코드 입력 후 `Shift + Enter`
- 텍스트 셀: 마크다운 문법으로 입력

| 단축키 | 설명 |
|--------|------|
| Shift + Enter | 현재 셀 실행 + 다음 셀 이동 |
| Ctrl + M + B | 아래에 코드 셀 추가 |
| Ctrl + M + M | 셀을 마크다운으로 변경 |

---

## 3. 파일 입출력

### 📂 Google Drive 연동

```python
from google.colab import drive
drive.mount('/content/drive')
