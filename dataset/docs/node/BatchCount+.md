- `BatchCount+`: The BatchCount+ node is designed to count the number of elements in a batch. It can handle various data structures, including tensors, dictionaries, and lists, making it versatile for different types of batched data.
    - Parameters:
    - Inputs:
        - `batch`: The 'batch' parameter represents the batch of data whose size is to be counted. It can be a tensor, a dictionary containing 'samples', or a list, accommodating a wide range of data structures. Type should be `*`.
    - Outputs:
        - `int`: This output represents the count of elements in the input batch, providing a straightforward way to determine the batch size. Type should be `INT`.
