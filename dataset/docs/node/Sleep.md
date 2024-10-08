- `Sleep`: Delays the execution for the input amount of time, allowing for a pause in operations based on specified minutes and seconds.
    - Parameters:
        - `minutes`: Specifies the duration of the delay in whole minutes, contributing to the total delay time alongside seconds. Type should be `INT`.
        - `seconds`: Specifies the duration of the delay in fractional minutes (seconds), fine-tuning the total delay time in conjunction with minutes. Type should be `FLOAT`.
    - Inputs:
        - `input`: A placeholder input that is returned after the delay, ensuring the flow of data is maintained throughout the node's operation. Type should be `*`.
    - Outputs:
        - `*`: Returns the input data unchanged after the specified delay, serving as a pass-through with a time delay. Type should be `*`.
