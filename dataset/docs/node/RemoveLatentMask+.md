- `RemoveLatentMask+`: This node is designed to process latent representations by removing any existing noise mask from the samples. It ensures that the latent samples are clean and devoid of any artificially added noise, making them suitable for further processing or generation tasks.
    - Parameters:
    - Inputs:
        - `samples`: The latent representation of an image or a batch of images. This input is crucial as it contains the data from which the noise mask, if present, will be removed. Type should be `LATENT`.
    - Outputs:
        - `latent`: The cleaned latent representation after the removal of the noise mask. This output is ready for further processing or generation tasks without the interference of previously added noise. Type should be `LATENT`.
