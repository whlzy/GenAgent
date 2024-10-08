- `SDXLEmptyLatentSizePicker+`: This node is designed to generate a tensor representing an empty latent space of a specified size, tailored for use in generative models. It allows for the dynamic creation of latent spaces based on resolution and batch size inputs, facilitating the generation of content at varying dimensions.
    - Parameters:
        - `resolution`: Specifies the resolution of the generated latent space, influencing the dimensions of the output tensor. The choice of resolution directly impacts the size and aspect ratio of the generated content. Type should be `COMBO[STRING]`.
        - `batch_size`: Determines the number of latent spaces to generate in a single batch, allowing for efficient bulk generation of content. Type should be `INT`.
    - Inputs:
    - Outputs:
        - `LATENT`: The generated empty latent space tensor, ready for further processing or generation tasks. Type should be `LATENT`.
        - `width`: The width dimension of the generated latent space, derived from the specified resolution. Type should be `INT`.
        - `height`: The height dimension of the generated latent space, derived from the specified resolution. Type should be `INT`.
