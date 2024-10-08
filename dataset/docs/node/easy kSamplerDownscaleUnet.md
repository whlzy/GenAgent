- `easy kSamplerDownscaleUnet`: This node specializes in dynamically adjusting the Unet model within a sampling pipeline, specifically targeting the downscaling of the model's dimensions to optimize performance and efficiency. It employs a methodical approach to modify the Unet configuration based on specific downscale factors, ensuring the model's output remains high-quality while potentially reducing computational load.
    - Parameters:
        - `downscale_mode`: Determines the mode of downscaling to be applied to the Unet model, allowing for automatic or manual adjustment of downscale parameters. Type should be `COMBO[STRING]`.
        - `block_number`: Specifies the block number within the Unet model to which the downscaling adjustments are applied, targeting specific layers for optimization. Type should be `INT`.
        - `downscale_factor`: The factor by which the Unet model's dimensions are reduced, directly influencing the model's performance and output quality. Type should be `FLOAT`.
        - `start_percent`: Defines the starting percentage of the model's operation range to begin downscaling, affecting the initial phase of model processing. Type should be `FLOAT`.
        - `end_percent`: Sets the ending percentage of the model's operation range for downscaling, impacting the final phase of model processing. Type should be `FLOAT`.
        - `downscale_after_skip`: A boolean flag indicating whether downscaling should occur after skip connections within the Unet model, affecting the model's internal architecture. Type should be `BOOLEAN`.
        - `downscale_method`: Specifies the method used for downscaling the Unet model, such as bicubic or nearest neighbor, influencing the quality of the downscaled output. Type should be `COMBO[STRING]`.
        - `upscale_method`: Determines the method used for upscaling within the Unet model, complementing the downscaling process to maintain output quality. Type should be `COMBO[STRING]`.
        - `image_output`: Controls the output format of the image, including options for preview, save, or hide, affecting the visibility and storage of the generated images. Type should be `COMBO[STRING]`.
        - `link_id`: An identifier for linking the current operation with other processes or outputs, facilitating the tracking and management of generated images. Type should be `INT`.
        - `save_prefix`: A prefix added to the filenames of saved images, allowing for organized storage and easy retrieval of generated content. Type should be `STRING`.
    - Inputs:
        - `pipe`: The pipeline through which the sampling process is executed, serving as the backbone for model operations and transformations. Type should be `PIPE_LINE`.
        - `model`: The model to be downscaled, typically a pre-loaded Unet model, which is the target of the downscaling adjustments. Type should be `MODEL`.
    - Outputs:
        - `pipe`: The updated pipeline after applying the downscaling adjustments, including any modifications to the model and processing parameters. Type should be `PIPE_LINE`.
        - `image`: The final image generated after the downscaling process, showcasing the effects of the applied adjustments on image quality and detail. Type should be `IMAGE`.
