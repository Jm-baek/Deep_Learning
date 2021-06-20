# Deep_learning

딥러닝의 기본이 되는 개념

### 참고 사이트  
  + 인프런 - 딥러닝 CNN 완벽 가이드 - Fundamental편

### 참고 서적
  + 밑바닥부터 시작하는 딥러닝 1


from tensorflow.keras.models import Sequential, Model <br/>
from tensorflow.keras.layers import Input, Dense , Conv2D , Dropout , Flatten , Activation, MaxPooling2D , GlobalAveragePooling2D  <br/>
from tensorflow.keras.optimizers import Adam , RMSprop <br/>
from tensorflow.keras.callbacks import **ReduceLROnPlateau**, EarlyStopping , ModelCheckpoint , LearningRateScheduler<br/>
from tensorflow.keras.preprocessing.image import ImageDataGenerator<br/>
