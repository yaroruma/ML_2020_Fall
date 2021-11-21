# ML_2020_Fall
## Brief
기계학습론 과목 개인 및 기말 팀 프로젝트 코드입니다. iPhone의 성능에 따른 다음 모델 예측을 위한 개인 프로젝트와 SECOM 데이터셋의 분류를 위한 기말 프로젝트로 이루어져있습니다.

## Personal project
아이폰 13이 나오기 전 시점에서 이전까지의 아이폰 모델들의 성능을 수치화하여 가격에 대한 regression 모델 제작 및 아이폰 13 가격 예측. 가격과 성능에 영향을 미치는 특성 분석.   
   
출시 전의 유출된 정보를 통해 하드웨어의 정보는 얻을 수 있지만 CPU의 벤치마크 점수등의 정보는 알 수 없으므로 벤치마크 점수를 먼저 예측하고 예측한 점수를 통해 가격 정보를 예측하도록 모델 제작. 비교를 위해 아이패드 8세대와 아이패드 에어의 정보를 통한 가격 예측도 진행.

### Environment
- Google Colab
- Scikit-learn

## Final project
SECOM 데이터셋을 이용한 반도체의 정상/불량 분류 모델 제작. 채점기준은 ROC-AUC score가 높은 순서로 순위 책정. 전처리 코드가 있었으나 심사 규정의 변화로 아주 간략하게 축소함.   
   
SGD classifier와 XGB classifier를 병행해서 사용. SGD classifier에서 성능이 더 좋았으므로 기본적으로 SGD classifier의 예측을 따라가지만, 의견의 불일치가 있을 때 XGB에서 확률이 높은 경우에는 XGB의 예측으로 바꾸는 선택적 voting 모델을 제작. 
### Environment
- Google Colab
- Scikit-learn
- XGBoost