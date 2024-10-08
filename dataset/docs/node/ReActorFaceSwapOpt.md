- `ReActorFaceSwapOpt`: This node specializes in offering optimized face swapping capabilities within the ReActor framework, providing users with advanced options for fine-tuning the face swap process. It extends the basic functionality of face swapping by incorporating additional parameters and optimizations to enhance the quality and flexibility of the output.
    - Parameters:
        - `enabled`: Determines whether the face swap operation is enabled or not, allowing users to toggle the functionality on demand. Type should be `BOOLEAN`.
        - `swap_model`: Specifies the model used for swapping faces, allowing selection from a predefined list of available models. Type should be `COMBO[STRING]`.
        - `facedetection`: Defines the face detection algorithm to be used, offering multiple options to best suit different image conditions. Type should be `COMBO[STRING]`.
        - `face_restore_model`: Selects the model for restoring face details post-swap, enhancing the overall quality of the swapped faces. Type should be `COMBO[STRING]`.
        - `face_restore_visibility`: Adjusts the visibility level of the restored face details, providing control over the blend between the original and restored face features. Type should be `FLOAT`.
        - `codeformer_weight`: Controls the influence of the CodeFormer model in the face restoration process, balancing between detail enhancement and naturalness. Type should be `FLOAT`.
    - Inputs:
        - `input_image`: The primary image input for the face swap operation, serving as the target for face replacement. Type should be `IMAGE`.
        - `source_image`: An optional secondary image input for the face swap, acting as the source of faces to be swapped into the primary image. Type should be `IMAGE`.
        - `face_model`: Optionally specifies a face model to be used in the swap, offering further customization of the swapping process. Type should be `FACE_MODEL`.
        - `options`: Provides additional configuration options for the face swap operation, allowing for more detailed customization. Type should be `OPTIONS`.
    - Outputs:
        - `image`: The output image after the face swap operation, featuring the swapped faces integrated into the original image. Type should be `IMAGE`.
        - `face_model`: Outputs the face model used in the swapping process, which can be utilized for further operations or analysis. Type should be `FACE_MODEL`.
