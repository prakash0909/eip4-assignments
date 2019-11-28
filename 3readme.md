Name : Prakash Shanmugam
Email : careers.prakash@gmail.com


Final Validation accuracy of base network is : 82.51


# Define the model
model = Sequential()
model.add(SeparableConv2D(32, (3, 3), activation='relu', kernel_initializer='he_uniform', padding='same', input_shape=(32, 32, 3)))  #32
model.add(BatchNormalization())
model.add(SeparableConv2D(32, (3, 3), activation='relu', kernel_initializer='he_uniform', padding='same'))  #32
model.add(BatchNormalization())
model.add(MaxPooling2D((2, 2)))  #16
model.add(Dropout(0.2))
model.add(SeparableConv2D(64, (3, 3), activation='relu', kernel_initializer='he_uniform', padding='same'))  #16
model.add(BatchNormalization())
model.add(SeparableConv2D(64, (3, 3), activation='relu', kernel_initializer='he_uniform', padding='same'))  #16
model.add(BatchNormalization())
model.add(MaxPooling2D((2, 2)))
model.add(Dropout(0.3))
model.add(SeparableConv2D(128, (3, 3), activation='relu', kernel_initializer='he_uniform', padding='same'))  #8
model.add(BatchNormalization())
model.add(SeparableConv2D(128, (3, 3), activation='relu', kernel_initializer='he_uniform', padding='same'))  #8
model.add(BatchNormalization())
model.add(MaxPooling2D((2, 2)))  #4
model.add(Dropout(0.4))
model.add(Flatten())
model.add(Dense(30, activation='relu', kernel_initializer='he_uniform'))
model.add(BatchNormalization())
model.add(Dropout(0.5))
model.add(Dense(num_classes, activation='softmax'))
# compile model
model.compile(optimizer='adam', loss='categorical_crossentropy', metrics=['accuracy'])




WARNING:tensorflow:From /usr/local/lib/python3.6/dist-packages/tensorflow_core/python/ops/math_grad.py:1424: where (from tensorflow.python.ops.array_ops) is deprecated and will be removed in a future version.
Instructions for updating:
Use tf.where in 2.0, which has the same broadcast rule as np.where
/usr/local/lib/python3.6/dist-packages/ipykernel_launcher.py:12: UserWarning: The semantics of the Keras 2 argument `steps_per_epoch` is not the same as the Keras 1 argument `samples_per_epoch`. `steps_per_epoch` is the number of batches to draw from the generator at each epoch. Basically steps_per_epoch = samples_per_epoch/batch_size. Similarly `nb_val_samples`->`validation_steps` and `val_samples`->`steps` arguments have changed. Update your method calls accordingly.
  if sys.path[0] == '':
/usr/local/lib/python3.6/dist-packages/ipykernel_launcher.py:12: UserWarning: Update your `fit_generator` call to the Keras 2 API: `fit_generator(<keras_pre..., validation_data=(array([[[..., verbose=1, shuffle=True, steps_per_epoch=390, epochs=50)`
  if sys.path[0] == '':
WARNING:tensorflow:From /usr/local/lib/python3.6/dist-packages/keras/backend/tensorflow_backend.py:1033: The name tf.assign_add is deprecated. Please use tf.compat.v1.assign_add instead.

WARNING:tensorflow:From /usr/local/lib/python3.6/dist-packages/keras/backend/tensorflow_backend.py:1020: The name tf.assign is deprecated. Please use tf.compat.v1.assign instead.

Epoch 1/50
390/390 [==============================] - 15s 39ms/step - loss: 1.9318 - acc: 0.3171 - val_loss: 1.4602 - val_acc: 0.4681
Epoch 2/50
390/390 [==============================] - 9s 23ms/step - loss: 1.4936 - acc: 0.4584 - val_loss: 1.2287 - val_acc: 0.5678
Epoch 3/50
390/390 [==============================] - 9s 24ms/step - loss: 1.3393 - acc: 0.5236 - val_loss: 1.1777 - val_acc: 0.5758
Epoch 4/50
390/390 [==============================] - 9s 24ms/step - loss: 1.2309 - acc: 0.5687 - val_loss: 1.0724 - val_acc: 0.6173
Epoch 5/50
390/390 [==============================] - 9s 23ms/step - loss: 1.1593 - acc: 0.5978 - val_loss: 0.9409 - val_acc: 0.6636
Epoch 6/50
390/390 [==============================] - 9s 23ms/step - loss: 1.0930 - acc: 0.6200 - val_loss: 0.9030 - val_acc: 0.6695
Epoch 7/50
390/390 [==============================] - 9s 23ms/step - loss: 1.0418 - acc: 0.6402 - val_loss: 1.0177 - val_acc: 0.6405
Epoch 8/50
390/390 [==============================] - 9s 23ms/step - loss: 0.9996 - acc: 0.6544 - val_loss: 0.8081 - val_acc: 0.7186
Epoch 9/50
390/390 [==============================] - 9s 24ms/step - loss: 0.9682 - acc: 0.6668 - val_loss: 0.7952 - val_acc: 0.7162
Epoch 10/50
390/390 [==============================] - 9s 23ms/step - loss: 0.9339 - acc: 0.6804 - val_loss: 0.7516 - val_acc: 0.7364
Epoch 11/50
390/390 [==============================] - 9s 24ms/step - loss: 0.9051 - acc: 0.6893 - val_loss: 0.8102 - val_acc: 0.7172
Epoch 12/50
390/390 [==============================] - 9s 23ms/step - loss: 0.8805 - acc: 0.6993 - val_loss: 0.7739 - val_acc: 0.7266
Epoch 13/50
390/390 [==============================] - 9s 24ms/step - loss: 0.8565 - acc: 0.7073 - val_loss: 0.7016 - val_acc: 0.7555
Epoch 14/50
390/390 [==============================] - 9s 23ms/step - loss: 0.8502 - acc: 0.7116 - val_loss: 0.7216 - val_acc: 0.7456
Epoch 15/50
390/390 [==============================] - 9s 24ms/step - loss: 0.8221 - acc: 0.7218 - val_loss: 0.6944 - val_acc: 0.7540
Epoch 16/50
390/390 [==============================] - 9s 24ms/step - loss: 0.8079 - acc: 0.7257 - val_loss: 0.7021 - val_acc: 0.7536
Epoch 17/50
390/390 [==============================] - 9s 24ms/step - loss: 0.7910 - acc: 0.7294 - val_loss: 0.6477 - val_acc: 0.7752
Epoch 18/50
390/390 [==============================] - 9s 23ms/step - loss: 0.7796 - acc: 0.7358 - val_loss: 0.6765 - val_acc: 0.7665
Epoch 19/50
390/390 [==============================] - 9s 24ms/step - loss: 0.7635 - acc: 0.7419 - val_loss: 0.6521 - val_acc: 0.7743
Epoch 20/50
390/390 [==============================] - 9s 24ms/step - loss: 0.7509 - acc: 0.7462 - val_loss: 0.6470 - val_acc: 0.7811
Epoch 21/50
390/390 [==============================] - 9s 23ms/step - loss: 0.7394 - acc: 0.7513 - val_loss: 0.6247 - val_acc: 0.7851
Epoch 22/50
390/390 [==============================] - 9s 23ms/step - loss: 0.7297 - acc: 0.7552 - val_loss: 0.6675 - val_acc: 0.7704
Epoch 23/50
390/390 [==============================] - 9s 24ms/step - loss: 0.7219 - acc: 0.7576 - val_loss: 0.6615 - val_acc: 0.7759
Epoch 24/50
390/390 [==============================] - 9s 24ms/step - loss: 0.7163 - acc: 0.7595 - val_loss: 0.6269 - val_acc: 0.7808
Epoch 25/50
390/390 [==============================] - 9s 24ms/step - loss: 0.7109 - acc: 0.7628 - val_loss: 0.5929 - val_acc: 0.7991
Epoch 26/50
390/390 [==============================] - 9s 23ms/step - loss: 0.6963 - acc: 0.7665 - val_loss: 0.6009 - val_acc: 0.7944
Epoch 27/50
390/390 [==============================] - 9s 24ms/step - loss: 0.6889 - acc: 0.7681 - val_loss: 0.5848 - val_acc: 0.7960
Epoch 28/50
390/390 [==============================] - 9s 23ms/step - loss: 0.6811 - acc: 0.7716 - val_loss: 0.5871 - val_acc: 0.8026
Epoch 29/50
390/390 [==============================] - 9s 24ms/step - loss: 0.6806 - acc: 0.7714 - val_loss: 0.6323 - val_acc: 0.7793
Epoch 30/50
390/390 [==============================] - 9s 24ms/step - loss: 0.6621 - acc: 0.7766 - val_loss: 0.5995 - val_acc: 0.7925
Epoch 31/50
390/390 [==============================] - 9s 24ms/step - loss: 0.6631 - acc: 0.7775 - val_loss: 0.5920 - val_acc: 0.7957
Epoch 32/50
390/390 [==============================] - 9s 24ms/step - loss: 0.6562 - acc: 0.7801 - val_loss: 0.6044 - val_acc: 0.7977
Epoch 33/50
390/390 [==============================] - 9s 24ms/step - loss: 0.6537 - acc: 0.7840 - val_loss: 0.5743 - val_acc: 0.8028
Epoch 34/50
390/390 [==============================] - 9s 23ms/step - loss: 0.6419 - acc: 0.7851 - val_loss: 0.5568 - val_acc: 0.8095
Epoch 35/50
390/390 [==============================] - 9s 24ms/step - loss: 0.6430 - acc: 0.7863 - val_loss: 0.5609 - val_acc: 0.8055
Epoch 36/50
390/390 [==============================] - 9s 23ms/step - loss: 0.6312 - acc: 0.7900 - val_loss: 0.6229 - val_acc: 0.7933
Epoch 37/50
390/390 [==============================] - 10s 25ms/step - loss: 0.6294 - acc: 0.7891 - val_loss: 0.5403 - val_acc: 0.8134
Epoch 38/50
390/390 [==============================] - 9s 24ms/step - loss: 0.6208 - acc: 0.7932 - val_loss: 0.5475 - val_acc: 0.8100
Epoch 39/50
390/390 [==============================] - 9s 23ms/step - loss: 0.6207 - acc: 0.7947 - val_loss: 0.5582 - val_acc: 0.8032
Epoch 40/50
390/390 [==============================] - 9s 23ms/step - loss: 0.6165 - acc: 0.7947 - val_loss: 0.5363 - val_acc: 0.8184
Epoch 41/50
390/390 [==============================] - 9s 23ms/step - loss: 0.6140 - acc: 0.7963 - val_loss: 0.5404 - val_acc: 0.8170
Epoch 42/50
390/390 [==============================] - 9s 23ms/step - loss: 0.6068 - acc: 0.7965 - val_loss: 0.5815 - val_acc: 0.8035
Epoch 43/50
390/390 [==============================] - 9s 23ms/step - loss: 0.6103 - acc: 0.7985 - val_loss: 0.5785 - val_acc: 0.8052
Epoch 44/50
390/390 [==============================] - 9s 23ms/step - loss: 0.6048 - acc: 0.8010 - val_loss: 0.5430 - val_acc: 0.8175
Epoch 45/50
390/390 [==============================] - 9s 24ms/step - loss: 0.5958 - acc: 0.8013 - val_loss: 0.5277 - val_acc: 0.8193
Epoch 46/50
390/390 [==============================] - 9s 23ms/step - loss: 0.5896 - acc: 0.8030 - val_loss: 0.5522 - val_acc: 0.8139
Epoch 47/50
390/390 [==============================] - 9s 23ms/step - loss: 0.5878 - acc: 0.8050 - val_loss: 0.5240 - val_acc: 0.8205
Epoch 48/50
390/390 [==============================] - 9s 23ms/step - loss: 0.5856 - acc: 0.8046 - val_loss: 0.5159 - val_acc: 0.8251
Epoch 49/50
390/390 [==============================] - 9s 24ms/step - loss: 0.5860 - acc: 0.8056 - val_loss: 0.5316 - val_acc: 0.8195
Epoch 50/50
390/390 [==============================] - 9s 23ms/step - loss: 0.5788 - acc: 0.8070 - val_loss: 0.5392 - val_acc: 0.8145
Model took 466.66 seconds to train

Accuracy on test data is: 81.45