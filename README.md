# Description

긴 맥락 대화에서의 감정인식을 위한 확장형 트랜스포머 소프트웨어

긴 맥락으로 구성된 대화에서 감정인식을 위해 발화 및 단어 간의 관계를 분석하는 어텐션을 분리하고
입력 크기를 늘려 긴 대화에서 감정인식을 가능하게 하는 모델을 통해 학습 비용을 줄이면서
긴 대화에서의 맥락 정보를 고려한다.

Environment

requirements.txt 참조

Files

requirements.txt - 환경
data.py - dataset load 코드
loss.py - loss 코드
model.py - model 코드
preprocessor.py - raw 데이터 전처리 코드,
train.py - 모델 훈련 코드
test.py - 모델 평가 코드
util.py - 각종 라이브러리, 예) min-max, mel spectogram

Usage

0. requirements.txt 참고하여 환경 설정
1. python preprocessor --data_pth '데이터 경로' - 데이터 경로에 raw 데이터 전처리 생성
2. python train.py - 학습 진행
3. python test.py - 평가 진행

이건 파일실행방법이야 이것도 포함해서 작성해주고 한글로 작성해줘

아래는 제공된 정보를 바탕으로 작성된 GitHub 프로젝트의 README 파일입니다. 한글로 작성되어 있으며, 실행 방법도 포함되어 있습니다.

---

# 긴 맥락 대화에서의 감정인식을 위한 확장형 트랜스포머

## **설명 (Description)**

이 프로젝트는 긴 맥락으로 구성된 대화에서 감정 인식을 수행하기 위한 확장형 트랜스포머 모델을 제공합니다.
발화 및 단어 간의 관계를 분석하는 어텐션을 분리하고 입력 크기를 늘려 긴 대화에서도 맥락 정보를 효과적으로 고려할 수 있도록 설계되었습니다.
이를 통해 학습 비용을 줄이면서도 높은 성능을 유지하며 감정 인식을 수행합니다.

---

## **환경 설정 (Environment)**

프로젝트 실행에 필요한 환경은 `requirements.txt` 파일에 정의되어 있습니다.
해당 파일을 참고하여 필요한 라이브러리를 설치하세요.

---

## **파일 설명 (Files)**

- **requirements.txt**: 프로젝트 실행에 필요한 환경 및 라이브러리 설정 파일
- **data.py**: 데이터셋 로드 코드
- **loss.py**: 손실 함수 관련 코드
- **model.py**: 모델 구조 코드
- **preprocessor.py**: 원시(raw) 데이터를 전처리하는 코드
- **train.py**: 모델 학습 코드
- **test.py**: 모델 평가 코드
- **util.py**: 다양한 유틸리티 함수 (예: min-max 정규화, mel spectrogram 생성 등)

---

## **사용 방법 (Usage)**

### 0. 환경 설정

`requirements.txt` 파일을 참고하여 필요한 라이브러리를 설치합니다. 아래 명령어를 사용하세요:

```bash
pip install -r requirements.txt
```


### 1. 데이터 전처리

원시 데이터를 전처리하여 학습에 적합한 형태로 변환합니다. 다음 명령어를 실행하세요:

```bash
python preprocessor.py --data_pth '데이터 경로'
```


### 2. 모델 학습

전처리된 데이터를 이용해 모델 학습을 진행합니다. 다음 명령어를 실행하세요:

```bash
python train.py
```


### 3. 모델 평가

학습된 모델을 평가하여 성능을 확인합니다. 다음 명령어를 실행하세요:

```bash
python test.py
```

---

## **참고사항**

1. 데이터 경로는 `--data_pth` 옵션을 통해 지정해야 합니다.
2. 모든 코드는 Python으로 작성되었으며, Python 3.x 버전을 사용하는 것을 권장합니다.
3. 학습 및 평가 시 GPU 사용을 권장하며, CUDA 환경이 필요할 수 있습니다.

---

이 README 파일을 GitHub 프로젝트의 루트 디렉토리에 저장하면 됩니다. 파일 이름은 `README.md`로 저장하세요! 추가적인 수정이나 문의 사항이 있다면 알려주세요! 😊

<div style="text-align: center">⁂</div>

[^1]: https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/56806610/f715c82f-ac4f-402a-a4d4-2d401487322b/gin-maegrag-daehwaeseoyi-gamjeonginsigeul-wihan-hwagjanghyeong-teuraenseupomeo-coejong.hwp

