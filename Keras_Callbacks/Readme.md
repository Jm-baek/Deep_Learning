## Keras Callbacks

    - 본 내용을 함부로 가져가서 사용하지 말아주세요!!
  
 본 내용은 인프런의 **딥러닝 CNN 완벽 가이드 - Fundamental 편** 을 듣고 요약한 내용입니다.


모델을 학습하다 보면 동적으로 learning rate 조절 또는 자동 저장 등을 하고 싶을 때가 있다.

이 때를 위해 우리가 사용할 수 있는 Keras의 Callback에 대해 알아보자!!

잘 사용하면 더 높은 성능을 찾을 수 있다. 

## Callback 종류
### Learning rate 동적 조절
- LearningRateScheduler
- ReduceLROnPlateau 


### EarlyStopping



### CheckPoint



## 주의 사항

#### keras의 batch 단위로 learning rate를 조절한다.
tf.keras.optimizers.LearningRateSchedule
예: model.compile(optimizer = Adame(learning_rate = CosineDecay()))  와 같이 copmile 호출 시 optimizer 인자로 입력

#### keras의 epochs 단위로 learning rate를 조절한다.
tf.keras.callbacks.LearningRateScheduler
model.fit(callbacks=[LearningRateScheduler(schedule_function)] 와 같이 fit 호출 시 callbacks 인자로 입력
