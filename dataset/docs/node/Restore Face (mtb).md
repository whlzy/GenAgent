- `Restore Face (mtb)`: The Restore Face node leverages GFPGan to enhance and restore faces in images, focusing on improving visual quality and details. It supports adjustments such as alignment, center face restoration, and weight modulation for tailored image enhancement.
    - Parameters:
        - `aligned`: A boolean indicating if the input faces are aligned. This affects how the model processes the image, potentially improving restoration quality for aligned faces. Type should be `BOOLEAN`.
        - `only_center_face`: A boolean that, when true, restricts the restoration to only the center face in the image, focusing the enhancement efforts. Type should be `BOOLEAN`.
        - `weight`: A float value representing the weight of the restoration effect. It allows for fine-tuning the intensity of the enhancement. Type should be `FLOAT`.
        - `save_tmp_steps`: A boolean indicating whether to save intermediate steps of the restoration process. This can be useful for debugging or analysis. Type should be `BOOLEAN`.
    - Inputs:
        - `image`: The input image tensor to be enhanced. It is crucial for the restoration process, determining the quality and focus of the enhancement. Type should be `IMAGE`.
        - `model`: The face enhancement model used for restoration. It defines the algorithm and parameters for the enhancement process. Type should be `FACEENHANCE_MODEL`.
    - Outputs:
        - `image`: The enhanced image tensor, showcasing improved facial details and overall image quality after restoration. Type should be `IMAGE`.
