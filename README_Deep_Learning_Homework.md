README: DEEP LEARNING ASSIGNMENT:
After building both models

> Which model has a lower loss?
>
FNG:
Real	Predicted
0	3670.919922	4331.251953
1	3670.919922	4292.001465
2	3912.570068	4233.851074
3	3924.239990	4741.745605
4	3974.050049	4784.239258

Loss
6/6 [==============================] - 2s 4ms/step - loss: 0.1805
0.18045997619628906

Model: "sequential_1"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 lstm_2 (LSTM)               (None, 1, 30)             3840      
                                                                 
 dropout_2 (Dropout)         (None, 1, 30)             0         
                                                                 
 lstm_3 (LSTM)               (None, 1, 30)             7320      
                                                                 
 dropout_3 (Dropout)         (None, 1, 30)             0         
                                                                 
 lstm_4 (LSTM)               (None, 30)                7320      
                                                                 
 dense (Dense)               (None, 1)                 31        
                                                                 
=================================================================
Total params: 18,511
Trainable params: 18,511
Non-trainable params: 0
_____________________________________



lmst: Stock Predictor:
Real	Predicted
2019-02-20	3924.239990	3886.710693
2019-02-21	3974.050049	3908.610840
2019-02-22	3937.040039	3935.941162
2019-02-23	3983.530029	3962.277832
2019-02-24	4149.089844	3986.018555

Loss:
5/5 [==============================] - 2s 4ms/step - loss: 0.0810
0.08102522045373917

Model: "sequential"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 lstm (LSTM)                 (None, 10, 30)            3840      
                                                                 
 dropout (Dropout)           (None, 10, 30)            0         
                                                                 
 lstm_1 (LSTM)               (None, 10, 30)            7320      
                                                                 
 dropout_1 (Dropout)         (None, 10, 30)            0         
                                                                 
 lstm_2 (LSTM)               (None, 30)                7320      
                                                                 
 dropout_2 (Dropout)         (None, 30)                0         
                                                                 
 dense (Dense)               (None, 1)                 31        
                                                                 
=================================================================
Total params: 18,511
Trainable params: 18,511
Non-trainable params: 0

