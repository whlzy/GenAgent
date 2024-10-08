- `PreviewLatentAdvanced`: This node is designed for advanced latent image preview generation, allowing for customization of the base model, preview method, and inclusion of additional metadata. It serves as a foundational component for generating previews of latent images with enhanced flexibility and control over the preview generation process.
    - Parameters:
        - `base_model`: Specifies the base model to use for preview generation, offering options between 'SD15' and 'SDXL' to adjust the preview quality and characteristics. Type should be `COMBO[STRING]`.
        - `preview_method`: Determines the method used for converting the latent representation to an image preview, with options including 'auto', 'taesd', and 'latent2rgb' for varied preview styles. Type should be `COMBO[STRING]`.
    - Inputs:
        - `latent`: The latent representation of an image to be previewed. It is a crucial component for generating the image preview. Type should be `LATENT`.
    - Outputs:
        - `latent`: Returns the latent representation of the image, maintaining consistency with the input while potentially incorporating modifications from the preview process. Type should be `LATENT`.
