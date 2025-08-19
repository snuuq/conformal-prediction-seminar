# Conformal Prediction Seminar
> 2025 Fall seminar on "[Theoretical Foundations of Conformal Prediction](https://arxiv.org/abs/2411.11824)"

## 일정표

| 주차  | 일자       | 내용                                                     | 담당자 |
| --- | -------- | ------------------------------------------------------ | --- |
| 1주  | 08. 25. | Ch2. Exchangeability and Permutations                  | 윤다연 |
| 2주  | 09. 01.   | Ch3. Conformal Prediction Under Exchangeability        | 이혜림 |
| 3주  | 09. 08.   | Ch4. Conditional Coverage                              | 박성희 |
| 4주  | 09. 15.   | Ch5. A Model-Based Perspective on Conformal Prediction | 변희준 |
| 5주  | 09. 22.   | Ch6. Cross-Validation Based Conformal Methods          | 최윤서 |
| 6주  | 09. 29.   | Ch7. Weighted Variants of Conformal Prediction         | 김지광 |
| 7주  | 10. 13.   | Ch8. Online Conformal Prediction                       | 박성우 |
| 8주  | 10. 27.   | Ch9. Additional Results in Conformal Prediction        | 윤다연 |
| 9주  | 11. 03.   | Ch10. Extensions of Conformal Prediction               | 이혜림 |
| 10주 | 11. 10.   | Ch11. Inference on the Regression Function             | 박성희 |
| 11주 | 11. 17.   | Ch12. Calibration                                      | 변희준 |
| 12주 | 11. 24.   | Ch13. Conditional Independence Testing                 | 최윤서 |

> 추석, 중간고사 일정을 반영해 간격을 조정했습니다. 추후 진도 사항에 따라 일정이 변경될 수 있습니다.

## 📋 세미나 규칙

- **매주 내용 읽기**
- **토요일까지** 주차 Issue에 질문 한개 이상 작성
- 해당 주차 담당자의 경우 **Issue에 작성된 질문들을 포함해 요약 발표 자료 작성**

## 사용법

### 1. Repository Clone

```bash
git clone https://github.com/snuuq/conformal-prediction-seminar.git
cd conformal-prediction-seminar
```

### 2. 해당 챕터 폴더 생성

```bash
mkdir ch02
```

챕터 폴더 포멧: `chXX` (XX는 챕터 번호)

### 3. 문제 풀이 후 업로드

```bash
# 1. 작업 시작 전에 최신 상태로 업데이트
git pull origin main

# 2. 파일 생성 및 자료 작성
touch ch02/main.tex
# OR
code .

# 3. 커밋 & 푸시
git add .
git commit -m "feat: ch02 presentation upload"
git push origin main
```

> 어렵다면 [Github Desktop](https://github.com/apps/desktop?locale=ko-KR)을 이용하거나 Github Web의 'Add file' 기능을 이용하세요.

