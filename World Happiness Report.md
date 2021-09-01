# World Happiness Report



## 변수 설명

| 변수명                                      | 속성   | 구분     |
| ------------------------------------------- | ------ | -------- |
| Country name(나라 이름)                     | 명목형 | Index    |
| year(연도)                                  | 순서형 | Index    |
| Life Ladder(행복 점수)                      | 연속형 | 종속변수 |
| Log GDP per capita(인당 국내 총생산 로그)   | 연속형 | 독립변수 |
| Social support(사회적 지원)                 | 연속형 | 독립변수 |
| Freedom to make life choices(삶의 자율성)   | 연속형 | 독립변수 |
| Generosity(복지에 대한 관대)                | 연속형 | 독립변수 |
| Perceptions of corruption(부패에 대한 인식) | 연속형 | 독립변수 |
| Positive affect(긍정적인 영향)              | 연속형 | 독립변수 |
| Negative affect(부정적인 영향)              | 연속형 | 독립변수 |



## 전처리

### 변수별 결측치 처리 방법

- Log GDP per capita(인당 국내 총생산 로그) : 결측치 전년도 다음년도 평균으로 대체
- Social support(사회적 지원) : 결측치 전년도 다음년도 평균으로 대체
- Freedom to make life choices(삶의 자율성) : 평균으로 대체
- Generosity(복지에 대한 관대) : 평균으로 대체
- Perceptions of corruption(부패에 대한 인식) : 평균으로 대체
- Positive affect(긍정적인 영향) : 평균으로 대체
- Negative affect(부정적인 영향) : 평균으로 대체

### 전처리 길라잡이

* 국가별로 결측치를 대체해야하기때문에 국가별로 데이터를 나눠야 함
* 국가 중 레코드의 수가 5개 이하인 국가는 삭제 처리
* 국가별로 데이터 프레임 생성하여 전처리 작업 수행
* 주변 평균치로 대체해야 하는 결측치는 이동평균 모듈 사용



## EDA

