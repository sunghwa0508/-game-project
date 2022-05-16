# 프로젝트 소개

1. [Game Analysis Project]
2. [Marketing Project]
3. [텍스트 분석을 위한 추천 서비스 구현]
4. [Anomaly Detection Project]



 해당 프로젝트는 유저 데이터를 바탕으로 인사이트도출 및 비즈니스적 의사결정을 하고 서비스를 구현하는 것을 목표로 하였습니다.


----------------------------------------------------------------------------------------------------------------------------------------------


# [Game Analysis Project]


<목적>

게임 회사의 데이터 팀에 합류하여 '다음 분기에 어떤 게임을 설계 해야 할까?'라는 고민을 해결하기 위해, 기존의 데이터에 기반하여 인사이트를 얻고 의사결정을 하고자 합니다.


<데이터셋 설명>

1980~2020년도의 게임데이터에 관한 정보로 게임명, 플랫폼, 장르, 제작사, 미국,영국,일본, 기타 나라별 게임 판매량에 대한 데이터를 가지고있습니다.

<설치 및 실행 방법>

확장자가 .py 및 .ipynb인 파일로 python환경에서 구현

<결과>

1. 게임매출에 대한 정보를 지역별로 상관분석, 연도별, 장르별 등으로 시각화하여 트랜드분석.
2. 높은 출고량을 가지는 게임에 대해서 분산분석과 카이제곱검정을 실시하여 데이터 값들 간의 연관성을 알아냄.

[Nintendo가 Action이 주가 아닌 다른 다양한 장르를 출시했음에도 가장 높은 출고량을 보였듯이

특정 연도에 수요가 있는 장르를 예측하는 것이별도로 필요합니다.

또한 북미, 유럽, 기타 국가들은 1980년대부터 2020년까지 꾸준한 수요가 있던 Action을 장르로 출시를,
일본에서는 Role-Playing로 출시를 하는 전략을 세울 것을 추천드립니다.

+ Nintendo사의 플랫폼인 Wii와 DS는 2009~2011년에 한하여 일시적인 수요를 보여주므로.
따라서 PS2와 PS3을 통해 게임을 출시하는 것이가장 안정입니다.]




----------------------------------------------------------------------------------------------------------------------------------------------





# [Marketing Project] 다음 마케팅을 위한 최상의 전략도출

<목적>
다음 마케팅 캠페인을 위해 개선 할 최상의 전략을 찾는것을 주제로 프로젝트를 진행하였습니다.


<데이터셋 설명>
마케팅 이후의 예금 여부를 확인하는 문제이므로 분류 문제이므로 deposit을 base line으로 설정하였습니다.

0: 마케팅 이후 예금을 하지 않음
1: 마케팅 이후 예금을 함

<설치 및 실행 방법>

확장자가 .py 및 .ipynb인 파일로 python환경에서 구현


<결과>

*다음 캠페인 성공을 위한 중요한 항목은 deposit여부와 관계없이 대상자와의 접촉을 늘리는 것입니다.

*월 분석에 따라 가입자가 많은 4월부터 8월까지의 기간의 활동을 늘리고, (기준치를 감소시키는 9월에는 활동을 줄이는 것을 추천드립니다.)

*퇴직자, 실업자, 기술자, 행정, 서비스직의 예금자 수가 많았으므로 이들을 중심으로 마케팅 하는것이 효율적이어 보입니다.

*학력이 높을수록 가입자가 많은 경향이 있어 이에 따라 기존 마케팅 내용을 누구나 알기쉽도록 수정하거나 학력에 따른 타겟을 정하는것이

성공적인 마케팅에 도움이 될 것으로 보입니다.


----------------------------------------------------------------------------------------------------------------------------------------------
# [텍스트 분석을 통한 추천 서비스 구현]


<목적>

대상에 대한 데이터 수집을 위해 DNN(심층신경망)을 이용하여 TikTok 영상에 등장하는 객체를 인식하고,
텍스트 분석을 통해 유사한 TicTok 영상을 소개하는 시스템을 구현하고자 합니다.


<분석방법>

사용한 분석기법


1.DNN

딥러닝 분석기법에는 ANN, DNN, RNN, CNN 등이 있는데 여기서는 ANN과 DNN을 소개하고자 합니다.

먼저 ANN은 사람의 신경망 원리와 구조를 모방하여 만든 기계학습 알고리즘으로 사람의 뇌와 같이 신호를 받고, 그 신호가 임계값을 넘어서면 결과 신호를 전달하는 과정입니다. 하지만 ANN은 학습시간이 느리고, 과적합의 위험이 있어 이를 은닉층의 개수를 늘림으로 ANN의 단점을 보완한 딥뉴럴네트워크 DNN을 사용하여 영상을 분석하고자 합니다.



2.코사인 유사도를 이용하여 텍스트 유사도를 분석
코사인 유사도는 단어를 수치화하여 벡터로 나타낸 후 벡터 간의 코사인 각도를 이용하여 구할 수 있는 두 벡터의 유사도를 의미합니다.


<결과>
추천 시스템에 TicTok 사용자가 관심이 있는 영상의 닉네임을 입력하면 10개의 영상에 대한 영상의 닉네임과 주소를 얻을 수 있습니다. 
