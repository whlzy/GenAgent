- `MaskExpandBatch+`: The MaskExpandBatch node is designed to process a batch of masks, applying expansion or contraction operations to each mask in the batch. This node enables the modification of mask boundaries, either dilating (expanding) or eroding (contracting) them, based on specified parameters. It is particularly useful in image processing tasks where precise control over mask dimensions is required.
    - Parameters:
        - `size`: The 'size' parameter specifies the magnitude of the expansion or contraction. Positive values indicate expansion, while negative values indicate contraction, directly affecting the size of the masks. Type should be `INT`.
        - `method`: The 'method' parameter determines the technique used for expanding or contracting the masks, offering a choice between different algorithms for mask manipulation. Type should be `COMBO[STRING]`.
    - Inputs:
        - `mask`: The 'mask' parameter represents the input batch of masks to be processed. It is crucial for defining the masks on which the expansion or contraction operations will be applied, directly influencing the node's output. Type should be `MASK`.
    - Outputs:
        - `mask`: The output is a batch of masks that have been either expanded or contracted based on the provided parameters, suitable for further image processing applications. Type should be `MASK`.
