
Model Test Accuracy - 99.50%

No of Total Parameters : 14,568

print(score):[0.019374087103898638, 0.995]


Train on 60000 samples, validate on 10000 samples
Epoch 1/20

Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
60000/60000 [==============================] - 139s 2ms/step - loss: 0.5657 - acc: 0.8402 - val_loss: 0.0959 - val_acc: 0.9806
Epoch 2/20

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022744503.
60000/60000 [==============================] - 136s 2ms/step - loss: 0.2620 - acc: 0.9211 - val_loss: 0.0692 - val_acc: 0.9846
Epoch 3/20

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018315018.
60000/60000 [==============================] - 134s 2ms/step - loss: 0.2091 - acc: 0.9374 - val_loss: 0.0574 - val_acc: 0.9868
Epoch 4/20

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015329586.
60000/60000 [==============================] - 135s 2ms/step - loss: 0.1799 - acc: 0.9435 - val_loss: 0.0425 - val_acc: 0.9892
Epoch 5/20

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013181019.
60000/60000 [==============================] - 134s 2ms/step - loss: 0.1605 - acc: 0.9475 - val_loss: 0.0373 - val_acc: 0.9897
Epoch 6/20

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011560694.
60000/60000 [==============================] - 134s 2ms/step - loss: 0.1500 - acc: 0.9479 - val_loss: 0.0345 - val_acc: 0.9912
Epoch 7/20

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010295127.
60000/60000 [==============================] - 135s 2ms/step - loss: 0.1367 - acc: 0.9509 - val_loss: 0.0291 - val_acc: 0.9924
Epoch 8/20

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009279307.
60000/60000 [==============================] - 134s 2ms/step - loss: 0.1325 - acc: 0.9516 - val_loss: 0.0283 - val_acc: 0.9918
Epoch 9/20

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008445946.
60000/60000 [==============================] - 134s 2ms/step - loss: 0.1273 - acc: 0.9515 - val_loss: 0.0289 - val_acc: 0.9912
Epoch 10/20

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007749935.
60000/60000 [==============================] - 134s 2ms/step - loss: 0.1212 - acc: 0.9526 - val_loss: 0.0251 - val_acc: 0.9929
Epoch 11/20

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007159905.
60000/60000 [==============================] - 134s 2ms/step - loss: 0.1186 - acc: 0.9536 - val_loss: 0.0266 - val_acc: 0.9928
Epoch 12/20

Epoch 00012: LearningRateScheduler setting learning rate to 0.000665336.
60000/60000 [==============================] - 134s 2ms/step - loss: 0.1143 - acc: 0.9532 - val_loss: 0.0251 - val_acc: 0.9929
Epoch 13/20

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006213753.
60000/60000 [==============================] - 133s 2ms/step - loss: 0.1110 - acc: 0.9539 - val_loss: 0.0235 - val_acc: 0.9935
Epoch 14/20

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005828638.
60000/60000 [==============================] - 132s 2ms/step - loss: 0.1090 - acc: 0.9560 - val_loss: 0.0212 - val_acc: 0.9932
Epoch 15/20

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005488474.
60000/60000 [==============================] - 134s 2ms/step - loss: 0.1069 - acc: 0.9559 - val_loss: 0.0244 - val_acc: 0.9927
Epoch 16/20

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005185825.
60000/60000 [==============================] - 134s 2ms/step - loss: 0.1060 - acc: 0.9534 - val_loss: 0.0213 - val_acc: 0.9946
Epoch 17/20

Epoch 00017: LearningRateScheduler setting learning rate to 0.000491481.
60000/60000 [==============================] - 134s 2ms/step - loss: 0.1043 - acc: 0.9549 - val_loss: 0.0209 - val_acc: 0.9940
Epoch 18/20

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004670715.
60000/60000 [==============================] - 135s 2ms/step - loss: 0.1016 - acc: 0.9559 - val_loss: 0.0242 - val_acc: 0.9925
Epoch 19/20

Epoch 00019: LearningRateScheduler setting learning rate to 0.0004449718.
60000/60000 [==============================] - 135s 2ms/step - loss: 0.0990 - acc: 0.9563 - val_loss: 0.0210 - val_acc: 0.9938
Epoch 20/20

Epoch 00020: LearningRateScheduler setting learning rate to 0.000424869.
60000/60000 [==============================] - 134s 2ms/step - loss: 0.1011 - acc: 0.9548 - val_loss: 0.0194 - val_acc: 0.9950
<keras.callbacks.History at 0x7f3ca4f31cc0>


Strategy: As per instructions added "use_bias=False" in all the convolution layers and changed number of filters from 16 to 8 in the fourth convolution layer thus helped me to achieve desired goal.

