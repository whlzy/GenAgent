- `BLIPCaption`: The `BLIPCaption` node is designed to generate textual captions for images using the BLIP model. It leverages deep learning techniques to analyze visual content and produce descriptive, human-like text based on the image's elements and context. This node can be customized with prefixes and suffixes to the generated captions, and it supports adjusting the length of the output text to fit specific requirements.
    - Parameters:
        - `min_length`: Specifies the minimum length of the generated caption. This parameter helps in ensuring that the captions are not too brief and convey sufficient detail. Type should be `INT`.
        - `max_length`: Sets the maximum length of the caption. This constraint ensures that the generated text is concise and to the point, avoiding overly verbose descriptions. Type should be `INT`.
        - `device_mode`: Determines the device (CPU or GPU) on which the BLIP model will run, optimizing performance based on the available hardware. Type should be `COMBO[STRING]`.
        - `prefix`: An optional text to prepend to the generated caption, allowing for additional context or information to be included. Type should be `STRING`.
        - `suffix`: An optional text to append to the generated caption, useful for adding extra details or clarifications. Type should be `STRING`.
        - `enabled`: A flag to enable or disable the caption generation feature. When disabled, it returns a default caption structure. Type should be `BOOLEAN`.
    - Inputs:
        - `image`: The input image to be captioned. This is the primary data the node processes to generate a textual description. Type should be `IMAGE`.
        - `blip_model`: An optional pre-loaded BLIP model to be used for caption generation. If not provided, the node will load a model based on available checkpoints. Type should be `BLIP_MODEL`.
    - Outputs:
        - `caption`: The generated captions for the input images, enriched with optional prefixes and suffixes. These captions provide a textual representation of the visual content. Type should be `STRING`.
