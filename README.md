# EIP-Session-2

# Logs for 20 epochs
Train on 60000 samples, validate on 10000 samples
Epoch 1/20

Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
60000/60000 [==============================] - 10s 168us/step - loss: 0.4110 - acc: 0.9359 - val_loss: 0.0839 - val_acc: 0.9848
Epoch 2/20

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022744503.
60000/60000 [==============================] - 7s 120us/step - loss: 0.1061 - acc: 0.9820 - val_loss: 0.0503 - val_acc: 0.9885
Epoch 3/20

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018315018.
60000/60000 [==============================] - 7s 120us/step - loss: 0.0747 - acc: 0.9848 - val_loss: 0.0494 - val_acc: 0.9865
Epoch 4/20

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015329586.
60000/60000 [==============================] - 7s 120us/step - loss: 0.0625 - acc: 0.9864 - val_loss: 0.0346 - val_acc: 0.9918
Epoch 5/20

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013181019.
60000/60000 [==============================] - 7s 120us/step - loss: 0.0514 - acc: 0.9881 - val_loss: 0.0352 - val_acc: 0.9895
Epoch 6/20

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011560694.
60000/60000 [==============================] - 7s 120us/step - loss: 0.0457 - acc: 0.9894 - val_loss: 0.0274 - val_acc: 0.9926
Epoch 7/20

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010295127.
60000/60000 [==============================] - 7s 121us/step - loss: 0.0418 - acc: 0.9899 - val_loss: 0.0336 - val_acc: 0.9892
Epoch 8/20

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009279307.
60000/60000 [==============================] - 7s 120us/step - loss: 0.0382 - acc: 0.9906 - val_loss: 0.0250 - val_acc: 0.9926
Epoch 9/20

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008445946.
60000/60000 [==============================] - 7s 120us/step - loss: 0.0357 - acc: 0.9911 - val_loss: 0.0222 - val_acc: 0.9934
Epoch 10/20

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007749935.
60000/60000 [==============================] - 7s 120us/step - loss: 0.0338 - acc: 0.9915 - val_loss: 0.0230 - val_acc: 0.9934
Epoch 11/20

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007159905.
60000/60000 [==============================] - 7s 121us/step - loss: 0.0328 - acc: 0.9917 - val_loss: 0.0185 - val_acc: 0.9944
Epoch 12/20

Epoch 00012: LearningRateScheduler setting learning rate to 0.000665336.
60000/60000 [==============================] - 7s 120us/step - loss: 0.0305 - acc: 0.9925 - val_loss: 0.0177 - val_acc: 0.9945
Epoch 13/20

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006213753.
60000/60000 [==============================] - 7s 120us/step - loss: 0.0289 - acc: 0.9925 - val_loss: 0.0194 - val_acc: 0.9936
Epoch 14/20

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005828638.
60000/60000 [==============================] - 7s 120us/step - loss: 0.0283 - acc: 0.9925 - val_loss: 0.0180 - val_acc: 0.9941
Epoch 15/20

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005488474.
60000/60000 [==============================] - 7s 120us/step - loss: 0.0259 - acc: 0.9934 - val_loss: 0.0203 - val_acc: 0.9942
Epoch 16/20

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005185825.
60000/60000 [==============================] - 7s 119us/step - loss: 0.0255 - acc: 0.9930 - val_loss: 0.0185 - val_acc: 0.9947
Epoch 17/20

Epoch 00017: LearningRateScheduler setting learning rate to 0.000491481.
60000/60000 [==============================] - 7s 119us/step - loss: 0.0251 - acc: 0.9933 - val_loss: 0.0239 - val_acc: 0.9930
Epoch 18/20

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004670715.
60000/60000 [==============================] - 7s 121us/step - loss: 0.0250 - acc: 0.9934 - val_loss: 0.0173 - val_acc: 0.9946
Epoch 19/20

Epoch 00019: LearningRateScheduler setting learning rate to 0.0004449718.
60000/60000 [==============================] - 7s 120us/step - loss: 0.0253 - acc: 0.9933 - val_loss: 0.0185 - val_acc: 0.9946
Epoch 20/20

Epoch 00020: LearningRateScheduler setting learning rate to 0.000424869.
60000/60000 [==============================] - 7s 119us/step - loss: 0.0242 - acc: 0.9934 - val_loss: 0.0172 - val_acc: 0.9946



# Result of model.evaluate (on test data)

[0.017244721205625684, 0.9946]

# Strategy taken to achieve the said results

1. Added a 1x1 layer before the last bach normalisation and dropout layers. This will help in effectively extracting the required features.
2. Used Global Average Pooling layer insted of flatten layer. This will help in effective extraction of feature values.

3.The total learnable parameter for the network is 14588 and non learnable parameter is 252. Total 14840 paramter with an validation accuracy of 99.46% after 20 epochs 

