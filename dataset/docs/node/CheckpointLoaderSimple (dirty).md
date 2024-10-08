- `CheckpointLoaderSimple (dirty)`: The CheckpointLoaderSimple (dirty) node is designed to streamline the process of loading model checkpoints in a less conventional or 'dirty' manner. It simplifies the checkpoint loading process by automatically finding and utilizing the appropriate checkpoint file based on a given name, facilitating easier and quicker model initialization for various applications.
    - Parameters:
        - `ckpt_name`: The 'ckpt_name' parameter specifies the name of the checkpoint file to be loaded. This node automates the process of finding the matching filename, making it easier to load models without needing to specify the exact file path. Type should be `STRING`.
    - Inputs:
    - Outputs:
        - `model`: The 'model' output represents the loaded model from the specified checkpoint, ready for further use or analysis. Type should be `MODEL`.
        - `clip`: The 'clip' output provides the CLIP model associated with the loaded checkpoint, if available and requested. Type should be `CLIP`.
        - `vae`: The 'vae' output delivers the VAE model linked with the loaded checkpoint, if available and requested. Type should be `VAE`.
