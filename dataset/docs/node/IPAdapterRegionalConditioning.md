- `IPAdapterRegionalConditioning`: The IPAdapterRegionalConditioning node is designed to apply regional conditioning to images using IPAdapter techniques. It focuses on enhancing or altering specific regions of an image based on given conditions, potentially including alternative conditions, unconditional inputs, and various weighting and masking strategies. This node plays a crucial role in customizing image processing tasks by allowing for detailed control over how different areas of an image are treated, making it essential for tasks that require precise adjustments or enhancements.
    - Parameters:
        - `image_weight`: Defines the weight of the image in the conditioning process, influencing the balance between the image and the conditioning effects. Type should be `FLOAT`.
        - `prompt_weight`: Specifies the weight of the prompt in the conditioning process, affecting the influence of textual conditions on the image. Type should be `FLOAT`.
        - `weight_type`: unknown Type should be `COMBO[STRING]`.
        - `start_at`: Indicates the starting point in the process where the conditioning begins to take effect, allowing for phased application. Type should be `FLOAT`.
        - `end_at`: Defines the ending point in the process where the conditioning ceases, enabling precise control over the duration of the effect. Type should be `FLOAT`.
    - Inputs:
        - `image`: The image to which regional conditioning will be applied, serving as the primary subject for the conditioning process. Type should be `IMAGE`.
        - `mask`: unknown Type should be `MASK`.
        - `positive`: A set of positive conditions under which the regional conditioning is applied, guiding the enhancements or adjustments. Type should be `CONDITIONING`.
        - `negative`: A set of negative conditions that the regional conditioning aims to mitigate or alter, providing a counterbalance to the positive conditions. Type should be `CONDITIONING`.
    - Outputs:
        - `IPADAPTER_PARAMS`: The parameters configured for the IPAdapter, detailing how the image and conditions are processed together. Type should be `IPADAPTER_PARAMS`.
        - `POSITIVE`: The modified set of positive conditions after the conditioning process, reflecting the applied enhancements. Type should be `CONDITIONING`.
        - `NEGATIVE`: The modified set of negative conditions after the conditioning process, reflecting the mitigated or altered aspects. Type should be `CONDITIONING`.
