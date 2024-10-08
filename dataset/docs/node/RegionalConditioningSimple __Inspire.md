- `RegionalConditioningSimple __Inspire`: This node specializes in applying regional conditioning to a given input, utilizing a combination of text prompts and masks to influence the generation process in specific areas. It integrates text encoding and mask application to create conditioned inputs tailored to regional specifications.
    - Parameters:
        - `strength`: Determines the intensity of the conditioning effect within the specified region. Type should be `FLOAT`.
        - `set_cond_area`: Specifies the method for setting the conditioning area, either to the default or based on mask bounds. Type should be `COMBO[STRING]`.
        - `prompt`: The text prompt used for generating the conditioning. This is encoded using the CLIP model. Type should be `STRING`.
    - Inputs:
        - `clip`: Represents the CLIP model used for encoding the text prompt into a format suitable for conditioning. Type should be `CLIP`.
        - `mask`: A mask that defines the area within the input where the conditioning should be applied. Type should be `MASK`.
    - Outputs:
        - `conditioning`: The output is a conditioned input, ready for further processing or generation tasks, tailored to the specified regional conditions. Type should be `CONDITIONING`.
