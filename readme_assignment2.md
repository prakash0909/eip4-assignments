Name : Prakash Shanmugam
Email : careers.prakash@gmail.com

LOGS FOR 20 EPOCHS 

Train on 60000 samples, validate on 10000 samples
Epoch 1/20

Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
60000/60000 [==============================] - 156s 3ms/step - loss: 0.6051 - acc: 0.8307 - val_loss: 0.1293 - val_acc: 0.9783
Epoch 2/20

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022744503.
60000/60000 [==============================] - 149s 2ms/step - loss: 0.2836 - acc: 0.9080 - val_loss: 0.0625 - val_acc: 0.9873
Epoch 3/20

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018315018.
60000/60000 [==============================] - 149s 2ms/step - loss: 0.2240 - acc: 0.9289 - val_loss: 0.0523 - val_acc: 0.9890
Epoch 4/20

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015329586.
60000/60000 [==============================] - 147s 2ms/step - loss: 0.1944 - acc: 0.9374 - val_loss: 0.0418 - val_acc: 0.9911
Epoch 5/20

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013181019.
60000/60000 [==============================] - 148s 2ms/step - loss: 0.1747 - acc: 0.9420 - val_loss: 0.0396 - val_acc: 0.9904
Epoch 6/20

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011560694.
60000/60000 [==============================] - 145s 2ms/step - loss: 0.1558 - acc: 0.9464 - val_loss: 0.0363 - val_acc: 0.9916
Epoch 7/20

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010295127.
60000/60000 [==============================] - 148s 2ms/step - loss: 0.1471 - acc: 0.9479 - val_loss: 0.0292 - val_acc: 0.9924
Epoch 8/20

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009279307.
60000/60000 [==============================] - 147s 2ms/step - loss: 0.1395 - acc: 0.9496 - val_loss: 0.0290 - val_acc: 0.9919
Epoch 9/20

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008445946.
60000/60000 [==============================] - 146s 2ms/step - loss: 0.1345 - acc: 0.9513 - val_loss: 0.0275 - val_acc: 0.9927
Epoch 10/20

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007749935.
60000/60000 [==============================] - 148s 2ms/step - loss: 0.1285 - acc: 0.9524 - val_loss: 0.0261 - val_acc: 0.9923
Epoch 11/20

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007159905.
60000/60000 [==============================] - 149s 2ms/step - loss: 0.1267 - acc: 0.9511 - val_loss: 0.0237 - val_acc: 0.9938
Epoch 12/20

Epoch 00012: LearningRateScheduler setting learning rate to 0.000665336.
60000/60000 [==============================] - 149s 2ms/step - loss: 0.1230 - acc: 0.9520 - val_loss: 0.0235 - val_acc: 0.9929
Epoch 13/20

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006213753.
60000/60000 [==============================] - 148s 2ms/step - loss: 0.1197 - acc: 0.9527 - val_loss: 0.0236 - val_acc: 0.9930
Epoch 14/20

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005828638.
60000/60000 [==============================] - 149s 2ms/step - loss: 0.1165 - acc: 0.9534 - val_loss: 0.0246 - val_acc: 0.9933
Epoch 15/20

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005488474.
60000/60000 [==============================] - 148s 2ms/step - loss: 0.1145 - acc: 0.9532 - val_loss: 0.0217 - val_acc: 0.9939
Epoch 16/20

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005185825.
60000/60000 [==============================] - 148s 2ms/step - loss: 0.1111 - acc: 0.9548 - val_loss: 0.0236 - val_acc: 0.9929
Epoch 17/20

Epoch 00017: LearningRateScheduler setting learning rate to 0.000491481.
60000/60000 [==============================] - 149s 2ms/step - loss: 0.1104 - acc: 0.9539 - val_loss: 0.0208 - val_acc: 0.9943
Epoch 18/20

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004670715.
60000/60000 [==============================] - 148s 2ms/step - loss: 0.1105 - acc: 0.9535 - val_loss: 0.0248 - val_acc: 0.9930
Epoch 19/20

Epoch 00019: LearningRateScheduler setting learning rate to 0.0004449718.
60000/60000 [==============================] - 149s 2ms/step - loss: 0.1086 - acc: 0.9537 - val_loss: 0.0222 - val_acc: 0.9938
Epoch 20/20

Epoch 00020: LearningRateScheduler setting learning rate to 0.000424869.
60000/60000 [==============================] - 148s 2ms/step - loss: 0.1061 - acc: 0.9553 - val_loss: 0.0201 - val_acc: 0.9945
<keras.callbacks.History at 0x7f1b35e9e978>


RESULT OF MODEL.EVALUATE

[0.020117798616783693, 0.9945]



STRATEGY FOLLOWED TO ACHIEVE THE RESULT

1. Used biases in all convolution layers.
2. Used seperable convolution technique. 5X5 = 5X1 and 1X5


