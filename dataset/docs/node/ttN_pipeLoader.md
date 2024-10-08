- `ttN pipeLoader`: The `ttN pipeLoader` node is designed to initialize and manage the loading process for various data pipelines within the tinyterraNodes framework. It abstracts the complexities involved in setting up and configuring the data flow, ensuring seamless integration and efficient handling of data across different stages of the pipeline.
    - Parameters:
        - `ckpt_name`: unknown Type should be `COMBO[STRING]`.
        - `config_name`: unknown Type should be `COMBO[STRING]`.
        - `vae_name`: unknown Type should be `COMBO[STRING]`.
        - `clip_skip`: unknown Type should be `INT`.
        - `lora1_name`: unknown Type should be `COMBO[STRING]`.
        - `lora1_model_strength`: unknown Type should be `FLOAT`.
        - `lora1_clip_strength`: unknown Type should be `FLOAT`.
        - `lora2_name`: unknown Type should be `COMBO[STRING]`.
        - `lora2_model_strength`: unknown Type should be `FLOAT`.
        - `lora2_clip_strength`: unknown Type should be `FLOAT`.
        - `lora3_name`: unknown Type should be `COMBO[STRING]`.
        - `lora3_model_strength`: unknown Type should be `FLOAT`.
        - `lora3_clip_strength`: unknown Type should be `FLOAT`.
        - `positive`: Defines the positive conditioning input for the pipeline, influencing the direction and nature of the data processing. Type should be `STRING`.
        - `positive_token_normalization`: unknown Type should be `COMBO[STRING]`.
        - `positive_weight_interpretation`: unknown Type should be `COMBO[STRING]`.
        - `negative`: Sets the negative conditioning input, providing a counterbalance to the positive conditioning and further refining the pipeline's output. Type should be `STRING`.
        - `negative_token_normalization`: unknown Type should be `COMBO[STRING]`.
        - `negative_weight_interpretation`: unknown Type should be `COMBO[STRING]`.
        - `empty_latent_width`: unknown Type should be `INT`.
        - `empty_latent_height`: unknown Type should be `INT`.
        - `batch_size`: unknown Type should be `INT`.
        - `seed`: Sets the seed for random number generation, ensuring reproducibility and consistency in the pipeline's operations. Type should be `INT`.
    - Inputs:
        - `model_override`: unknown Type should be `MODEL`.
        - `clip_override`: unknown Type should be `CLIP`.
        - `optional_lora_stack`: unknown Type should be `LORA_STACK`.
    - Outputs:
        - `pipe`: Outputs the configured pipeline, ready for further processing or analysis. Type should be `PIPE_LINE`.
        - `model`: Outputs the model component of the pipeline. Type should be `MODEL`.
        - `positive`: Outputs the positive conditioning component of the pipeline. Type should be `CONDITIONING`.
        - `negative`: Outputs the negative conditioning component of the pipeline. Type should be `CONDITIONING`.
        - `latent`: Outputs the latent space representation used in the pipeline. Type should be `LATENT`.
        - `vae`: Outputs the VAE model integrated into the pipeline. Type should be `VAE`.
        - `clip`: Outputs the CLIP model component of the pipeline. Type should be `CLIP`.
        - `seed`: Outputs the seed used for random number generation in the pipeline. Type should be `INT`.
