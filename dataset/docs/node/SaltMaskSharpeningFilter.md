- `SaltMaskSharpeningFilter`: This node applies a sharpening filter to a collection of masks, enhancing their edges and details according to a specified strength. It's designed to refine mask visuals by iteratively applying a sharpening effect, making the features within the masks more pronounced.
    - Parameters:
        - `strength`: Defines the intensity of the sharpening effect. A higher value results in a more pronounced sharpening effect on the masks. Type should be `INT`.
    - Inputs:
        - `masks`: The collection of masks to be sharpened. This input is crucial for determining the regions within which the sharpening filter will be applied. Type should be `MASK`.
    - Outputs:
        - `MASKS`: The output is a tensor of sharpened masks, where each mask has undergone the specified number of sharpening iterations to enhance its details. Type should be `MASK`.
