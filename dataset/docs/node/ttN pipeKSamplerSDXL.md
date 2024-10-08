- `ttN pipeKSamplerSDXL`: The `ttN_pipeKSamplerSDXL` node is designed for advanced image sampling, leveraging a sophisticated pipeline to enhance image generation with specific configurations and enhancements. It integrates various components such as LoRA adjustments, noise control, and optional model inputs to tailor the image generation process, aiming to produce high-quality images with fine-tuned characteristics.
    - Parameters:
        - `upscale_method`: Specifies the method used for upscaling images, affecting the resolution and quality of the output images. Type should be `COMBO[STRING]`.
        - `factor`: Determines the scaling factor for upscaling, directly influencing the final image size and detail level. Type should be `FLOAT`.
        - `crop`: Defines the cropping parameters to apply to the generated images, adjusting the composition and focus areas. Type should be `COMBO[STRING]`.
        - `sampler_state`: Indicates the current state of the sampler, guiding the flow of the sampling process and determining the next steps. Type should be `COMBO[STRING]`.
        - `base_steps`: Specifies the number of steps for the base sampling process, affecting the detail and quality of the generated images. Type should be `INT`.
        - `refiner_steps`: Determines the number of steps for the refining process, enhancing the final image quality through additional adjustments. Type should be `INT`.
        - `cfg`: Controls the CFG (Classifier Free Guidance) scale, influencing the adherence to the input prompts and the overall image quality. Type should be `FLOAT`.
        - `sampler_name`: Identifies the specific sampler algorithm to be used, affecting the sampling behavior and output characteristics. Type should be `COMBO[STRING]`.
        - `scheduler`: Specifies the scheduler for controlling the sampling process, impacting the progression and adjustments during image generation. Type should be `COMBO[STRING]`.
        - `image_output`: Determines the output format and handling of the generated images, including saving and displaying options. Type should be `COMBO[STRING]`.
        - `save_prefix`: Sets the prefix for saved image files, organizing and identifying the outputs. Type should be `STRING`.
        - `seed`: Provides a seed for the random number generator, ensuring reproducibility of the generated images. Type should be `INT`.
    - Inputs:
        - `sdxl_pipe`: Represents the current state of the sampling pipeline, including configurations and intermediate results, which is essential for continuing or adjusting the image generation process. Type should be `PIPE_LINE_SDXL`.
        - `optional_model`: Allows for the specification of an alternative model for image generation, offering flexibility in the sampling process. Type should be `MODEL`.
        - `optional_positive`: Enables the use of alternative positive prompts, adjusting the thematic direction of the generated images. Type should be `CONDITIONING`.
        - `optional_negative`: Permits the specification of alternative negative prompts, refining the avoidance criteria in the image generation. Type should be `CONDITIONING`.
        - `optional_vae`: Provides an option to use an alternative VAE model, affecting the encoding and decoding of images. Type should be `VAE`.
        - `optional_refiner_model`: Allows for the use of a different model for refining the generated images, enhancing the final output quality. Type should be `MODEL`.
        - `optional_refiner_positive`: Enables the use of alternative positive prompts for the refining process, further guiding the image enhancement. Type should be `CONDITIONING`.
        - `optional_refiner_negative`: Permits the specification of alternative negative prompts for the refining process, fine-tuning the avoidance criteria. Type should be `CONDITIONING`.
        - `optional_refiner_vae`: unknown Type should be `VAE`.
        - `optional_latent`: Provides an option to specify an alternative latent representation, influencing the starting point of the generation process. Type should be `LATENT`.
        - `optional_clip`: Allows for the use of an alternative CLIP model, affecting the alignment between text prompts and generated images. Type should be `CLIP`.
    - Outputs:
        - `sdxl_pipe`: Outputs the updated state of the sampling pipeline, including any changes or results from the current sampling operation. Type should be `PIPE_LINE_SDXL`.
        - `model`: Returns the model used in the sampling process, potentially updated or altered based on optional inputs. Type should be `MODEL`.
        - `positive`: Provides the positive prompts used in the image generation, reflecting any optional adjustments. Type should be `CONDITIONING`.
        - `negative`: Returns the negative prompts guiding the avoidance criteria in the image generation. Type should be `CONDITIONING`.
        - `vae`: Outputs the VAE model involved in the encoding and decoding of images during the sampling process. Type should be `VAE`.
        - `refiner_model`: Provides the model used for refining the generated images, potentially updated or altered based on optional inputs. Type should be `MODEL`.
        - `refiner_positive`: Returns the positive prompts used in the refining process, reflecting any optional adjustments. Type should be `CONDITIONING`.
        - `refiner_negative`: Provides the negative prompts used in the refining process, guiding the avoidance criteria. Type should be `CONDITIONING`.
        - `refiner_vae`: unknown Type should be `VAE`.
        - `latent`: Outputs the latent representation of the generated images, central to the image generation and refinement processes. Type should be `LATENT`.
        - `clip`: Returns the CLIP model used to align text prompts with the generated images, potentially updated based on optional inputs. Type should be `CLIP`.
        - `image`: Provides the final generated images, showcasing the results of the sampling and refining processes. Type should be `IMAGE`.
        - `seed`: Outputs the seed used in the random number generator, ensuring reproducibility of the generated images. Type should be `INT`.
