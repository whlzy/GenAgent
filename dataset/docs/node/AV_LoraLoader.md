- `AV_LoraLoader`: The AV_LoraLoader node is designed to load and apply LoRA (Low-Rank Adaptation) models to given models and CLIP instances, optionally overriding the default LoRA model with a specified one and enabling or disabling the loading process. This functionality enhances model customization and flexibility in processing, allowing for dynamic adjustments and optimizations based on specific requirements or preferences.
    - Parameters:
        - `lora_name`: Specifies the name of the LoRA model to be loaded and applied, enabling targeted modifications to the base model and CLIP instance. Type should be `COMBO[STRING]`.
        - `strength_model`: Specifies the strength of the LoRA adjustment to be applied to the model, allowing for fine-tuned control over the adaptation process. Type should be `FLOAT`.
        - `strength_clip`: Specifies the strength of the LoRA adjustment to be applied to the CLIP model, enabling precise customization of the enhancement. Type should be `FLOAT`.
        - `lora_override`: Allows for the specification of an alternative LoRA model to override the default, providing flexibility in model customization. Type should be `STRING`.
        - `enabled`: A boolean flag that determines whether the LoRA loading and application process should be executed, offering control over the modification workflow. Type should be `BOOLEAN`.
    - Inputs:
        - `model`: The model parameter represents the neural network model to which the LoRA adjustments will be applied, serving as the base for modifications. Type should be `MODEL`.
        - `clip`: The clip parameter signifies the CLIP model that will be adjusted alongside the main model, allowing for synchronized enhancements in processing capabilities. Type should be `CLIP`.
    - Outputs:
        - `model`: Returns the modified neural network model with applied LoRA adjustments, reflecting the enhancements or customizations made. Type should be `MODEL`.
        - `clip`: Returns the modified CLIP model with applied LoRA adjustments, showcasing the enhancements or customizations made to processing capabilities. Type should be `CLIP`.
