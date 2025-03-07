# 경험시차의 발생 여부 확인 {#sec:research-table}


<!-- Table formatting works same as figure formatting -->

[@tbl:random] shows us how to add a table. Integer tincidunt sed nisl eget pellentesque. Mauris eleifend, nisl non lobortis fringilla, sapien eros aliquet orci, vitae pretium massa neque eu turpis. Pellentesque tincidunt aliquet volutpat. Ut ornare dui id ex sodales laoreet.

<!-- Force the table onto a newpage -->

\newpage

-----------------------------------------------------------------------------------
Landmass      \%      Number of   Dolphins per    How Many     How Many    Forbidden
             stuff    Owls        Capita         Foos         Bars        Float
------------ ------- --------- -------------- ------------ ------------ -----------
    North       94%    20,028       17,465        12,084       20,659       1.71
 America                                                               

Central      91%     6564         6350         8,189        12,012       1.52
America                                                               

    South       86%     3902         4127         5,205        6,565        1.28
America                                                               

    Africa      84%     2892         3175         3,862        4,248         1.1

    Europe      92%    20,964       17,465        15,303       24,203       1.58

    Asia       87%     6852         6350         8,255        11,688       1.47

Oceania      87%     4044         4127         5,540        6,972        1.28

Antarctica    83%     2964         3175         4,402        4,941        1.13
-----------------------------------------------------------------------------------

: Important data for various land masses. []{#tbl:random short-caption="Table short caption"}

## 분석 결과

이 연구에서는 도로명주소 정책에 경험시차가 발생하고 있는지를 통계적으로 검증하기 위하여 통계 패키지(R)를 이용하여 2017년~2019년 서울시 도로명주소 여론조사 결과의 원본 데이터를 분석하였다. 분석 대상 질문은 주소 정책의 인지도, 사용 경험, 사용 빈도, 도로명주소를 사용한 경험이 있는 영역, 도로명주소에 불만족하는 응답자의 경우 그 이유, 아직까지 지번주소를 사용한다고 생각하는 영역이 어디인지이며, 이러한 질문에 대하여 2017년과 2018년, 2018년과 2019년의 응답에 통계적으로 유의한 차이가 있는지를 ANOVA 방법 및 T-test를 통하여 확인하였다. 그 결과는 다음 [표 5-1]과 같다. 2014년~2016년은 원본 데이터가 없으므로 통계 검증 대상은 아니나, 응답결과 수치 변화의 참고를 위하여 일부 문항에 대해서는 그 결과를 그래프에 함께 표시하였다.

[표 5-1] 서울시 도로명주소 여론조사 결과(2017~2019) 분석 결과

## 결과의 해석

### 본인 집의 도로명주소 인지도

본인 집의 도로명주소를 정확히 알고 있는지를 묻는 질문에 대하여 정확히 알고 있다고 답한 응답자의 비율은 2017년 79.7%에서 2018년 83%, 2019년 85.3%로 증가하였다. 본인 집의 인지도를 1=정확히 앎, 2=어렴풋이 앎, 3=모름으로 점수화하여 T-test를 수행한 결과 2017년-2018년 간 인지도 증가만 통계적으로 유의한 것으로 나타났다.

1. 도로명과 건물번호로 이루어진 “00로 00” 또는 “00로00길 00” 형태의
도로명주소로 된 선생님 댁의 집 주소를 알고 계십니까? 

![그림 5-1 문항 1번에 대한 응답 결과<br>출처: 서울특별시 여론조사(research.seoul.go.kr) 자료를 활용하여 저자 작성](source/figures/page_73_img_1.png){#fig5-1 width=100% .center short-caption=""}

### 도로명주소 사용 경험

2017년부터 2019년까지 모두 길을 찾거나 알려줄 때, 우편물이나 택배를 보낼 때, 주민등록 등 민원서류를 발급받을 때 등 실생활에서 도로명주소를 사용해 본 경험이 있는 응답자의 비율은 90% 이상인 것으로 나타났다.

2. 선생님께서는 길을 찾거나 알려줄 때, 우편물이나 택배를 보낼 때, 주
민등록 등 민원서류를 발급받을 때 등 실생활에서 도로명주소를 사용
해 본 경험이 있으십니까?

![그림 5-2 문항 2번에 대한 응답 결과<br>출처: 서울특별시 여론조사(research.seoul.go.kr) 자료를 활용하여 저자 작성](source/figures/page_73_img_2.png){#fig5-2 width=100% .center short-caption=""}

### 도로명주소 사용 빈도

도로명주소와 지번주소 가운데 도로명주소를 주로 사용한다고 답한 응답자의 비율은 2017년 46.5%에서 2018년 54.7%, 2019년에는 60.5%로 증가하였다. 도로명주소 사용 빈도를 1=도로명주소, 2=혼용(도로명>지번), 3=혼용(도로명<지번), 4=지번주소로 점수화하여 T-test를 수행한 결과는 도로명주소 사용 빈도가 2017년과 2018년, 2018년과 2019년이 동일하다는 귀무가설을 각각 기각하므로 도로명주소 사용 빈도가 연도별로 증가한다는 결론을 뒷받침하였다. 다만 도로명주소 정책의 목표는 국민들이 실생활의 모든 분야에서 ISO의 주소의 정의에 입각한 식별과 위치찾기라는 주소의 제 기능을 활용하는 데 무리가 없는 환경을 만드는 것이라는 점에서 ‘주로 도로명주소를 사용한다’의 응답율을 올리는 데 걸리는 시간을 단축할 수 있는 정책수단이 필요하다.

3. 선생님께서는 평소 도로명주소를 얼마나 자주 사용하시나요?(’17~’19)

![그림 5-3 문항 3번에 대한 응답 결과<br>출처: 서울특별시 여론조사(research.seoul.go.kr) 자료를 활용하여 저자 작성](source/figures/page_74_img_1.png){#fig5-3 width=100% .center short-caption=""}

### 상황별 도로명주소 사용 경험

상황별 도로명주소 사용 경험에 대하여는, 연도별 해당 상황에서의 경험이 있는 응답자 수 변화 여부가 보기 항목별로 차이가 있었다. 먼저 1. 길을 찾거나 위치를 알려줄 때, 6. 음식 등을 배달시킬 때 도로명주소를 사용한 경험이 있다고 한 응답자의 비율은 2017년에 비하여 2018년, 2019년에 증가하였다. 

2. 우편물이나 택배 등을 보낼 때, 3. 홈페이지 회원가입 시 주소를 작성할 때, 4. 주민등록등본 등 민원서류를 발급할 때, 5. 내비게이션 검색할 때 도로명주소를 사용한 경험이 있다고 응답한 응답자의 비율은 2017년과 2018년은 큰 차이가 없으나 2019년에는 증가하였다.

이 문항에서 주목할 점은 1. 길을 찾거나 위치를 알려줄 때, 5. 내비게이션 검색할 때, 6. 음식 등을 배달시킬 때와 같이 생활 속에서 도로명주소를 사용하는 경험이 있는 비율이 50%를 밑돌고 있다는 점이다. 특히 이 문항의 질문이 위와 같은 상황에서 도로명주소를 ‘주로’ 사용하는지가 아닌, 단순히 도로명주소를 사용해 본 ‘경험이 있는지’를 물어본 것인데도 응답률이 50%를 밑돈다는 것은 실제로 위와 같은 상황에서 도로명주소를 사용하는 국민의 비율은 더 낮다는 사실을 의미하기 때문이다.

4. 선생님께서는 아래와 같은 상황에서 도로명주소를 사용하십니까? 도
로명주소를 사용해 본 상황을 모두 선택해 주십시오. (복수응답)(’19)

![그림 5-4 문항 4번에 대한 응답 결과<br>※ 선생님께서는 도로명주소를 어디에 사용해 보셨습니까? (복수응답)(’15~’18)<br>※ 선생님께서는 직접 도로명주소를 사용해 보신적이 있으십니까?(길을 찾거나,우편물 또는 택배 발송, 주민등록등본 등 민원서류를 발급 등)(’14)<br>출처: 서울특별시 여론조사(research.seoul.go.kr) 자료를 활용하여 저자 작성](source/figures/page_76_img_1.png){#fig5-4 width=100% .center short-caption=""}

### 도로명주소 사용 만족도

도로명주소 사용에 대한 만족도는 2017년 63%의 응답자가 ‘매우 만족한다’ 또는 ‘만족한다’고 응답하였으며, 이 비율은 2018년 71%, 2019년 75.7%로 증가하였다. 1=매우 만족, 2=만족, 3=만족하지 않음, 4=매우 만족하지 않음으로 점수화하여 T-test를 수행한 결과, 2017년-2018년 간, 2018-2019년 간 만족도 증가가 모두 통계적으로 유의하였다.

5. 선생님께서는 도로명주소 사용에 어느 정도 만족하십니까?

![그림 5-5 문항 5번에 대한 응답 결과<br>출처: 서울특별시 여론조사(research.seoul.go.kr) 자료를 활용하여 저자 작성](source/figures/page_77_img_1.png){#fig5-5 width=100% .center short-caption=""}

### 도로명주소 불만족 이유

5번 문항에서 도로명주소 사용에 대하여 불만족스럽다고 답한 응답자들은 도로명주소 사용에 대하여 불만족하다고 생각한 이유에 대하여 ‘주소를 들어도 위치를 알기 어렵다’, ‘익숙하지 않아 불편하다’, ‘주소를 기억하기가 어렵다’, ‘도로명주소 체계를 이해하기 어렵다’, ‘집이나 건물을 찾아가기 어렵다’, ‘지번주소를 요구하는 경우가 있다’, ‘주소 검색이나 조회가 잘 되지 않는다’ 순으로 응답하였다. 이러한 응답에 대하여 연도별 T-test를 수행한 결과, 응답 비율이 연도별로 감소하는 경향은 없는 것으로 나타났다. 이는 2017~19년 3년 간 연도별로 도로명주소 자체의 인지도와 만족도는 올라가고는 있으나, 도로명주소 정책의 한계점을 극복하기 위한 정부의 노력은 국민에게 체감되지 않고 있음을 보여준다.

응답 가운데 ‘도로명주소 체계를 이해하기 어렵다’, ‘집이나 건물을 찾아가기 어렵다’라는 응답이 연도별로 감소하지 않는 것은 김태승 등(2015)이 지적하였듯이 도로명주소의 원리에 대한 교육과 정책체험의 기회가 시간이 지나도 부족한 점이 그 원인일 수 있다. 일례로 종속구간에 위치한 건물의 길찾기를 들 수 있는데, 정부는 해당 구간에 건물이 10개동 미만이거나, 도로구간의 길이가 짧거나, 막다른길인 구간은 별도의 도로명을 부여하지 않고 인접한 도로의 종속구간으로 설정하여 건물번호에 가지번호(예: 13-24, 610-2 등)를 부여할 수 있도록 하고 있다. 상당수의 지자체가 도로구간을 경제적으로 설정하기 위하여 종속구간을 과도하게 많이 설정하였고, 이로 인하여 종속구간에 위치하여 가지번호로 된 주소를 갖는 건물은 기하급수적으로 많아졌다. 그렇다면 종속구간의 개념을 국민들에게 정확히 알려야 국민들이 그 원리를 이해하고 도로명주소로 위치찾기에 활용할 수 있는데, 그럼에도 불구하고 이에 대한 홍보는 미흡한 측면이 있었다. 이런 점 때문에 국민들은 자신이 도로명주소 체계에 대한 이해가 부족하다고 느끼거나, 도로명주소로 집이나 건물을 찾아가는 데 어려움이 있는 것이다.

행정안전부 담당자 인터뷰 시 이에 대하여 질문한 결과, 정부도 종속구간 등 도로명주소 부여 원리에 대한 심도 있는 대국민 교육이 부족했다는 점을 인지는 하고 있었다. 아래는 도로명주소 원리에 대한 대국민교육과 관련한 행정안전부 주소정책과 관계자의 인터뷰 답변이다.

_“정부도 기초번호의 부여 원리(종속구간 가지번호 부여 등 포함)를 포함하여 도로명주소의 상세한 원리, 확장성, 적용 방법에 대한 대국민교육의 필요성을 인지는 하고 있으나, 전 국민 대상으로 홍보를 하다보니 국민들이 느낄 내용상의 부담을 우려하여 불가피하게 기초 수준의 원리만 반복하여 교육해 왔습니다.”_(5.26. 행정안전부 주소정책과 관계자(D 사무관) 인터뷰)

_“우리나라 도로명주소가 기초번호를 기반으로 하다 보니 확장성이 좋다는 특징이 있습니다. 그렇기 때문에 건물은 아니지만 사람들이 많이 이용하는 거리가게나 육교 승강기 등 사물주소, 푸드트럭과 같이 이동하는 물체에도 기초번호를 활용하여 실시간으로 주소를 부여할 수 있습니다. 최근 주소 정책의 취지는 정부 주도에서 국민 중심으로 전환되고 있어서, 앞으로의 도로명주소는 기초번호를 보다 적극적으로 활용하는 주소체계로 나아갈 계획입니다.”_(4.14. 행정안전부 주소정책과 관계자(E 주무관) 인터뷰)

한편 응답 가운데 ‘익숙하지 않아 불편하다’, ‘주소를 기억하기가 어렵다’, ‘지번주소를 요구하는 경우가 있다’, ‘주소 검색이나 조회가 잘 되지 않는다’ 는 도로명주소의 표기와 관련되어 있다고 볼 수 있다. 도로명주소에서 띄어쓰기는 지번주소와 달리 엄격하게 지켜야 하는데, 그 이유는 아직 주소 검색 체계가 고도화되지 않은 채로 보급되어 있기 때문이다. 이 때문에 띄어쓰기를 지키지 않고 입력할 경우 조회가 안 되는 경우가 빈번하며, 도로명을 검색하기 위하여 행정구역을 선택하여야만 한다거나, 도로명의 정렬이 제각각인 문제도 발생한다. 이러한 불편사항은 본 문항의 기타 의견에서도 확인할 수 있다.

※ 기타 의견: “자동차 내비게이션에 도로명주소로 찾을 때 시간이 꽤 걸린다”, “OO 앱에서 특정 도로명을 선택하려면 스크롤을 200번씩 해야 한다”, “(택시, 배달 등에서) 도로명주소를 말해도 못 알아들을 때가 많아서 지번주소를 얘기해야 할 때가 있다.”, “인터넷 검색이 잘 안 된다(띄어쓰기 잘못하면 검색 안 됨)”, “온라인사이트에서 주소입력 시 검색 및 입력이 몇 배 오래 걸린다” 등

6. 선생님께서 도로명주소 사용에 불만족한 이유는 무엇입니까? 해당하
는 이유를 모두 선택해주십시오. (복수응답)

![그림 5-6 문항 6번에 대한 응답 결과<br>출처: 서울특별시 여론조사(research.seoul.go.kr) 자료를 활용하여 저자 작성](source/figures/page_80_img_1.png){#fig5-6 width=100% .center short-caption=""}

### 생활 속 도로명주소 사용 정도

생활 속에서 도로명주소를 어느 정도 사용하고 있다고 생각하냐는 질문에 대하여 1=대부분 사용, 2=대체로 사용, 3=별로 사용 안 함, 4=대부분 사용 안 함으로 가정했을 때, 2017년에는 71.4%, 2018년에는 81.5%, 2019년에는 78.8%의 응답자가 대부분 또는 대체로 사용한다고 응답하였다. 2017년에서 2018년은 소폭 증가하였지만 2018년에서 2019년은 소폭 감소하였으며 t-test 결과 이 결과는 통계적으로 유의한 것으로 나타났다.

7. 선생님께서는 우리 생활에서 얼마나 많은 사람들이 도로명주소를 사
용하고 있다고 느끼십니까?(’16~’19)

![그림 5-7 문항 7번에 대한 응답 결과<br>출처: 서울특별시 여론조사(research.seoul.go.kr) 자료를 활용하여 저자 작성](source/figures/page_81_img_1.png){#fig5-7 width=100% .center short-caption=""}

### 아직까지 지번주소를 사용하는 곳

아직까지 지번주소를 사용하는 곳에 대한 의견으로 응답자들은 배달 음식점, 택배 및 퀵서비스, 내비게이션 길 찾기 서비스, 온라인 쇼핑몰 순서대로 답하였다. 각 보기의 응답자 비율이 3개년도 평균을 벗어나는지 알아보기 위하여 ANOVA test를 실시한 결과, 이 중 배달 음식점, 택배 및 퀵서비스, 온라인 쇼핑몰의 응답자 비율은 평균을 벗어났다는 통계학적 증거가 없었다. 즉, 이 상태가 앞으로도 지속된다면 국민들은 도로명주소 사용의 필요성에 대하여 인지하고 있으면서도 배달 음식점, 택배 및 퀵서비스, 온라인 쇼핑몰 등 생활 내 특정 분야에서는 여전히 지번주소를 혼용하게 되어 정책목표인 택배, 배달, 생활 속 길 안내 등 선진국 수준의 ‘실생활에서의 전면적인 사용’은 기약이 없어질 수도 있다. 배달 음식점, 택배 및 퀵서비스, 온라인 쇼핑몰 등 상황에서 국민들이 아직까지 지번주소를 사용하고 있다고 느끼는 이유에 대해서는 6번 문항의 기타 의견을 참고하여 추론할 수 있다.

[그림 5-8] 문항 8번에 대한 응답 결과

8. 도로명주소를 사용하지 않고 아직까지 지번주소를 주로 사용하는 곳이 어디라고 생각하십니까? (복수응답)(’15~’19)

![그림 5-8 문항 8번에 대한 응답 결과<br>출처: 서울특별시 여론조사(research.seoul.go.kr) 자료를 활용하여 저자 작성](source/figures/page_82_img_1.png){#fig5-8 width=100% .center short-caption=""}


## 소결 및 분석의 한계

### 소결

위 조사 결과로부터 도로명주소의 인지도와 사용경험, 사용빈도는 연도별로 증가하고 있으며 이는 통계적으로도 유의하다는 점을 알 수 있었다. 다만 상황별 도로명주소 사용 경험에서 사용하지 않는 분야의 경험자의 비율, 도로명주소에 대해 불만족하다고 생각하는 이유, 아직까지 지번주소를 사용하는 곳은 연도별로 다르다고 말할 통계적인 증거가 없었다. 이는 아직 주소 정책이 정책순응의 초기 단계로서 국민들이 도로명주소를 ‘식별 및 위치찾기’ 기능으로 활용하기 위한 학습효과가 발휘되지 못하는 단계라고 말할 수 있다. 이는 앞서 이 연구에서 우리나라 주소 정책이 본래 의도한 정책 목표를 국민들이 실생활 속 모든 분야에서 식별과 위치 찾기라는 주소의 제 기능을 제대로 활용하는 환경을 조성하는 것으로 설정하였으므로, 이러한 관점에서는 주소 정책에 대하여 김태승(2015)이 제안한 개념의 경험시차가 발생하고 있다고 결론 내릴 수 있다. 즉, 2020년 현재로서는 ‘불완전하게 이전된 정책’으로 판단할 수 있다.

### 분석의 한계

도로명주소 정책은 전 국민이 정책대상이므로 행정안전부 등 정부 차원의 전국 단위 조사 결과를 분석하거나 서울시 외 다른 지자체가 실시한 설문조사 결과를 함께 분석하는 것이 바람직하나, 이 연구에서는 다음과 같은 두 가지의 한계가 있어 서울시가 실시한 “도로명주소에 대한 시민인식 조사”만을 분석하였다. 첫째, “행정안전부가 주관하여 실시한 도로명주소 만족도 조사는 도로명주소가 어느 정도 정착이 되었다고 보고 중간에 질문 내용을 크게 바꾼 적이 있었기 때문에”[^26] 시간에 따라 변화하는 국민들의 인식을 알아내기는 목적으로 사용하기에는 부적합하다고 판단하였다. 서울시 설문조사는 질문의 구성이 2016년, 2017년에 일부 질문이 변경된 점, 2018년에 보기 1개가 추가된 점 외에는 2014년부터 구성이 변경되지 않았으며, 표본 수, 조사 방식 등이 일관되었다. 둘째, 2014년부터 2018년까지 부산광역시, 인천광역시(부평구), 대전광역시, 세종특별자치시, 경기도, 경기도(군포시), 전라북도(남원시), 경상남도 등 다른 지자체가 실시한 설문조사 결과를 인터넷으로 사전 조사한 결과, 대부분은 홍보 성격의 일회성 설문조사로서 서울시 설문조사와는 달리 연도별로 같은 질문으로 구성되어 있지 않았다. 연도별로 질문의 구성이 같더라도 해당 조사의 질문 구성은 서울시 설문조사보다 국민들의 인식도와 만족도, 개선 과제 등을 도출해 내기에 불충분하다고 판단되었다.

도로명주소 정책이 전 국민이 대상이므로 서울시 설문조사 결과만을 활용하는 것은 서울시민의 일반적인 특성에 따라 편향된 결론이 나올 수 있다는 점, 읍면 지역의 특성을 반영하지 못하는 점, 서울시가 일련번호방식의 도로명 부여 방식을 채택했다는 점에서 기초번호방식, 기타 방식의 도로명 부여 방식을 채택한 지자체의 특성을 반영하지 못하는 등의 한계가 있으나, 도로명주소에 대한 국민들의 인식도와 만족도가 연도별로 어떻게 변했는지 알아보고, 나아가 도로명주소 정책 관련 국민 불편요소를 발굴하며 해당 요소들이 연도별로 개선되었는지 파악하기 위한 분석으로서는 타당하다고 가정하고 분석을 진행하였다.

[^26]: 5.26. 행정안전부 주소정책과 관계자(D 사무관) 인터뷰.