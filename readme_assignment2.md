Name : Prakash Shanmugam
Email : careers.prakash@gmail.com

LOGS FOR 20 EPOCHS 

Train on 60000 samples, validate on 10000 samples
Epoch 1/20

Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
60000/60000 [==============================] - 141s 2ms/step - loss: 0.6312 - acc: 0.8225 - val_loss: 0.1164 - val_acc: 0.9808
Epoch 2/20

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022744503.
60000/60000 [==============================] - 137s 2ms/step - loss: 0.2946 - acc: 0.9041 - val_loss: 0.0663 - val_acc: 0.9868
Epoch 3/20

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018315018.
60000/60000 [==============================] - 137s 2ms/step - loss: 0.2303 - acc: 0.9270 - val_loss: 0.0506 - val_acc: 0.9890
Epoch 4/20

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015329586.
60000/60000 [==============================] - 136s 2ms/step - loss: 0.1919 - acc: 0.9389 - val_loss: 0.0492 - val_acc: 0.9900
Epoch 5/20

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013181019.
60000/60000 [==============================] - 138s 2ms/step - loss: 0.1728 - acc: 0.9438 - val_loss: 0.0354 - val_acc: 0.9924
Epoch 6/20

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011560694.
60000/60000 [==============================] - 138s 2ms/step - loss: 0.1596 - acc: 0.9462 - val_loss: 0.0410 - val_acc: 0.9900
Epoch 7/20

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010295127.
60000/60000 [==============================] - 138s 2ms/step - loss: 0.1508 - acc: 0.9464 - val_loss: 0.0308 - val_acc: 0.9917
Epoch 8/20

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009279307.
60000/60000 [==============================] - 139s 2ms/step - loss: 0.1401 - acc: 0.9496 - val_loss: 0.0282 - val_acc: 0.9931
Epoch 9/20

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008445946.
60000/60000 [==============================] - 138s 2ms/step - loss: 0.1340 - acc: 0.9514 - val_loss: 0.0302 - val_acc: 0.9924
Epoch 10/20

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007749935.
60000/60000 [==============================] - 138s 2ms/step - loss: 0.1271 - acc: 0.9526 - val_loss: 0.0262 - val_acc: 0.9933
Epoch 11/20

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007159905.
60000/60000 [==============================] - 138s 2ms/step - loss: 0.1212 - acc: 0.9543 - val_loss: 0.0249 - val_acc: 0.9932
Epoch 12/20

Epoch 00012: LearningRateScheduler setting learning rate to 0.000665336.
60000/60000 [==============================] - 138s 2ms/step - loss: 0.1200 - acc: 0.9527 - val_loss: 0.0237 - val_acc: 0.9931
Epoch 13/20

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006213753.
60000/60000 [==============================] - 138s 2ms/step - loss: 0.1166 - acc: 0.9543 - val_loss: 0.0243 - val_acc: 0.9931
Epoch 14/20

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005828638.
60000/60000 [==============================] - 137s 2ms/step - loss: 0.1133 - acc: 0.9544 - val_loss: 0.0204 - val_acc: 0.9946
Epoch 15/20

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005488474.
60000/60000 [==============================] - 136s 2ms/step - loss: 0.1119 - acc: 0.9554 - val_loss: 0.0221 - val_acc: 0.9943
Epoch 16/20

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005185825.
60000/60000 [==============================] - 137s 2ms/step - loss: 0.1100 - acc: 0.9550 - val_loss: 0.0230 - val_acc: 0.9936
Epoch 17/20

Epoch 00017: LearningRateScheduler setting learning rate to 0.000491481.
60000/60000 [==============================] - 137s 2ms/step - loss: 0.1102 - acc: 0.9541 - val_loss: 0.0194 - val_acc: 0.9951
Epoch 18/20

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004670715.
60000/60000 [==============================] - 137s 2ms/step - loss: 0.1062 - acc: 0.9558 - val_loss: 0.0205 - val_acc: 0.9946
Epoch 19/20

Epoch 00019: LearningRateScheduler setting learning rate to 0.0004449718.
60000/60000 [==============================] - 137s 2ms/step - loss: 0.1043 - acc: 0.9561 - val_loss: 0.0195 - val_acc: 0.9946
Epoch 20/20

Epoch 00020: LearningRateScheduler setting learning rate to 0.000424869.
60000/60000 [==============================] - 137s 2ms/step - loss: 0.1041 - acc: 0.9554 - val_loss: 0.0206 - val_acc: 0.9944
<keras.callbacks.History at 0x7fb896085b00>


RESULT OF MODEL.EVALUATE

[0.020643361882469617, 0.9944]



STRATEGY FOLLOWED TO ACHIEVE THE RESULT

1. Removed biases in all convolution layers.
2. Removed one Convolution2D layer.
3. Used spatially seperable convolution technique. 5X5 = 5X1 and 1X5


