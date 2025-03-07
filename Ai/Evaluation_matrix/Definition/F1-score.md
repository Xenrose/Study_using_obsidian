# F1-Score

## 정의
* 정밀도(Precision)와 재현율(Recall)의 조화평균
	* Precision = TP / (TP+FP) << True로 예측한 것 중 진짜로 True인 비율
	* Recall = TP / (TP+FN) << 실제로 True인 것 중 True로 예측한 비율

	
## 공식 
$$F1-Score = 2 * \frac{(Precision * Recall)}{(Precision + Recall)}$$


## 해석
* 0~1 사이의 값이 출력되며 1에 가까울수록 좋은 성능


## 특징
1. 클래스 불균형이 존재하는 데이터에서 정확도보다 더 좋은 성능을 보임.


## 한계
1. True Negative를 고려하지 않음.
2. Precision과 Recall의 상대적 중요도를 고려하지 않음. (둘 다 동일한 가중치 적용)
3. 여전히 불균형 데이터에 대해서는 한계가 있음. (소수 클래스에 대한 예측이 틀릴 경우 Score가 크게 하락하지만, 다수 클래스의 예측이 틀리는 경우 상대적으로 영향이 작음.)

  
## 사용 예시
* 클래스 불균형이 존재하는 데이터
* 2진 분류 문제


