# Dacon_signlanguage

Dacon novice 수화 이미지 classification 

-DLA CNN 모델을 활용하여 전이학습을 함. 일부 layer은 얼리지 않고 진행 (Tree 4 Tree 5부분은 얼리지 않음) - 성능이 향상됨 

-이후 full layer 학습 시도, 시간이 오래걸렸지만 기존의 얼린 것과 동일한 성능 발휘 - 아마 overfitting 이 일어났으리라 추측 

-Data augmentation을 시도하였음. - Random rotation을 줌. flip은 제외함.- test image dataset을 보았을 때, 수화라는 이미지 특성상 반대로 뒤집힌 데이터는 안좋다고 생각함.

-valid set을 따로 두었지만, 이번엔 testset의 일부를 valid로 활용함 - model architecture에 비해 data개수가 작음. - 정확도 향상

결과 : 2022-05-26 오전 02시 기준 7등. (상위 7%)

소감 : 기본적인 EDA , train 과정이나 dataset 만드는 과정을 다시 복습하는 중. - Sota architecture을 나도 좋은 걸 만들어보고 싶다.



DLA model citation 

citation : 
{
https://github.com/ucbdrive/dla
}
