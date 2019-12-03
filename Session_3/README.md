Base Model Test Score: 0.8248 Total params: 1,172,410

Best Model Test Score: 0.8325, Total params: 84,27


Model Definition:

model = Sequential()

model.add(SeparableConv2D(48, 3, 3, border_mode='same', input_shape=(32, 32, 3))) # 32x32x48, 3

model.add(BatchNormalization()) 

model.add(Activation('relu')) 

model.add(SeparableConv2D(48, 3, 3)) # 30x30x48, 5

model.add(BatchNormalization())

model.add(Activation('relu'))

model.add(MaxPooling2D(pool_size=(2, 2))) # 15x15x48, 7

model.add(Dropout(0.1))

model.add(SeparableConv2D(96, 3, 3, border_mode='same')) # 15x15x96, 15

model.add(BatchNormalization())

model.add(Activation('relu'))

model.add(SeparableConv2D(96, 3, 3)) # 13x13x96, 23

model.add(BatchNormalization())

model.add(Activation('relu'))

model.add(MaxPooling2D(pool_size=(2, 2))) # 6x6x96, 27

model.add(Dropout(0.1))

model.add(SeparableConv2D(192, 3, 3, border_mode='same')) # 6x6x192 , 44

model.add(BatchNormalization())

model.add(Activation('relu'))

model.add(SeparableConv2D(192, 3, 3)) # 4x4x192 , 60

model.add(BatchNormalization())

model.add(Activation('relu'))

model.add(MaxPooling2D(pool_size=(2, 2))) # 2x2x192, 68

model.add(Dropout(0.1))

model.add(SeparableConv2D(num_classes, 4, border_mode='same')) # 2x2x10, 100

model.add(GlobalAveragePooling2D())

model.add(Activation('softmax')) 

# Compile the model

model.compile(optimizer='adam', loss='categorical_crossentropy', metrics=['accuracy'])


Model Epoch History:

Epoch 1/50
1562/1562 [==============================] - 62s 40ms/step - loss: 1.3817 - acc: 0.5046 - val_loss: 1.5076 - val_acc: 0.4896
Epoch 2/50
1562/1562 [==============================] - 59s 38ms/step - loss: 1.0612 - acc: 0.6258 - val_loss: 0.9780 - val_acc: 0.6550
Epoch 3/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.9535 - acc: 0.6669 - val_loss: 1.1161 - val_acc: 0.6296
Epoch 4/50
1562/1562 [==============================] - 59s 38ms/step - loss: 0.8861 - acc: 0.6920 - val_loss: 0.8974 - val_acc: 0.7009
Epoch 5/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.8366 - acc: 0.7076 - val_loss: 1.0314 - val_acc: 0.6662
Epoch 6/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.8037 - acc: 0.7199 - val_loss: 0.8087 - val_acc: 0.7221
Epoch 7/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.7786 - acc: 0.7288 - val_loss: 0.9165 - val_acc: 0.7044
Epoch 8/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.7503 - acc: 0.7373 - val_loss: 0.6879 - val_acc: 0.7631
Epoch 9/50
1562/1562 [==============================] - 59s 38ms/step - loss: 0.7335 - acc: 0.7440 - val_loss: 0.8046 - val_acc: 0.7277
Epoch 10/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.7089 - acc: 0.7531 - val_loss: 0.7068 - val_acc: 0.7616
Epoch 11/50
1562/1562 [==============================] - 59s 38ms/step - loss: 0.6932 - acc: 0.7601 - val_loss: 0.7684 - val_acc: 0.7396
Epoch 12/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.6844 - acc: 0.7615 - val_loss: 0.6528 - val_acc: 0.7722
Epoch 13/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.6649 - acc: 0.7679 - val_loss: 0.5896 - val_acc: 0.7989
Epoch 14/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.6585 - acc: 0.7710 - val_loss: 0.7791 - val_acc: 0.7444
Epoch 15/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.6474 - acc: 0.7755 - val_loss: 0.6935 - val_acc: 0.7644
Epoch 16/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.6411 - acc: 0.7779 - val_loss: 0.6434 - val_acc: 0.7807
Epoch 17/50
1562/1562 [==============================] - 62s 40ms/step - loss: 0.6298 - acc: 0.7810 - val_loss: 0.6067 - val_acc: 0.7928
Epoch 18/50
1562/1562 [==============================] - 61s 39ms/step - loss: 0.6205 - acc: 0.7850 - val_loss: 0.6833 - val_acc: 0.7754
Epoch 19/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.6124 - acc: 0.7870 - val_loss: 0.6924 - val_acc: 0.7736
Epoch 20/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.6054 - acc: 0.7884 - val_loss: 0.7188 - val_acc: 0.7667
Epoch 21/50
1562/1562 [==============================] - 59s 38ms/step - loss: 0.5916 - acc: 0.7959 - val_loss: 0.6355 - val_acc: 0.7880
Epoch 22/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.5940 - acc: 0.7941 - val_loss: 0.7295 - val_acc: 0.7590
Epoch 23/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.5822 - acc: 0.7981 - val_loss: 0.7424 - val_acc: 0.7627
Epoch 24/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.5796 - acc: 0.7989 - val_loss: 0.7138 - val_acc: 0.7718
Epoch 25/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.5722 - acc: 0.8026 - val_loss: 0.6098 - val_acc: 0.7967
Epoch 26/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.5649 - acc: 0.8015 - val_loss: 0.5634 - val_acc: 0.8114
Epoch 27/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.5600 - acc: 0.8046 - val_loss: 0.6632 - val_acc: 0.7866
Epoch 28/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.5612 - acc: 0.8045 - val_loss: 0.5973 - val_acc: 0.7990
Epoch 29/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.5537 - acc: 0.8086 - val_loss: 0.6138 - val_acc: 0.7968
Epoch 30/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.5497 - acc: 0.8094 - val_loss: 0.5847 - val_acc: 0.8031
Epoch 31/50
1562/1562 [==============================] - 59s 38ms/step - loss: 0.5413 - acc: 0.8105 - val_loss: 0.5941 - val_acc: 0.8058
Epoch 32/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.5392 - acc: 0.8139 - val_loss: 0.5760 - val_acc: 0.8115
Epoch 33/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.5329 - acc: 0.8153 - val_loss: 0.5107 - val_acc: 0.8300
Epoch 34/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.5353 - acc: 0.8132 - val_loss: 0.5222 - val_acc: 0.8257
Epoch 35/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.5307 - acc: 0.8150 - val_loss: 0.5825 - val_acc: 0.8120
Epoch 36/50
1562/1562 [==============================] - 59s 38ms/step - loss: 0.5212 - acc: 0.8175 - val_loss: 0.5824 - val_acc: 0.8124
Epoch 37/50
1562/1562 [==============================] - 59s 38ms/step - loss: 0.5184 - acc: 0.8185 - val_loss: 0.5506 - val_acc: 0.8203
Epoch 38/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.5186 - acc: 0.8209 - val_loss: 0.6226 - val_acc: 0.8001
Epoch 39/50
1562/1562 [==============================] - 59s 38ms/step - loss: 0.5087 - acc: 0.8231 - val_loss: 0.6055 - val_acc: 0.8020
Epoch 40/50
1562/1562 [==============================] - 59s 38ms/step - loss: 0.5058 - acc: 0.8254 - val_loss: 0.5817 - val_acc: 0.8131
Epoch 41/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.5041 - acc: 0.8239 - val_loss: 0.5491 - val_acc: 0.8166
Epoch 42/50
1562/1562 [==============================] - 59s 38ms/step - loss: 0.5067 - acc: 0.8235 - val_loss: 0.6078 - val_acc: 0.7998
Epoch 43/50
1562/1562 [==============================] - 59s 38ms/step - loss: 0.5053 - acc: 0.8245 - val_loss: 0.5316 - val_acc: 0.8231
Epoch 44/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.4986 - acc: 0.8273 - val_loss: 0.5573 - val_acc: 0.8138
Epoch 45/50
1562/1562 [==============================] - 59s 38ms/step - loss: 0.4940 - acc: 0.8275 - val_loss: 0.4767 - val_acc: 0.8414
Epoch 46/50
1562/1562 [==============================] - 59s 38ms/step - loss: 0.4940 - acc: 0.8293 - val_loss: 0.5949 - val_acc: 0.8108
Epoch 47/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.4946 - acc: 0.8282 - val_loss: 0.5376 - val_acc: 0.8187
Epoch 48/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.4888 - acc: 0.8304 - val_loss: 0.5399 - val_acc: 0.8213
Epoch 49/50
1562/1562 [==============================] - 60s 38ms/step - loss: 0.4823 - acc: 0.8312 - val_loss: 0.5381 - val_acc: 0.8264
Epoch 50/50
1562/1562 [==============================] - 59s 38ms/step - loss: 0.4830 - acc: 0.8325 - val_loss: 0.4998 - val_acc: 0.8325
Model took 2989.09 seconds to train


