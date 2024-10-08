- `IPAdapterLoadEmbeds`: The IPAdapterLoadEmbeds node is designed for loading pre-saved embedding vectors from files with a specific extension, facilitating the reuse of embeddings in image processing applications.
    - Parameters:
        - `embeds`: Specifies the file names from which to load the embeddings, enabling the selection of specific pre-saved embeddings for use in the node's operation. Type should be `COMBO[STRING]`.
    - Inputs:
    - Outputs:
        - `embeds`: Returns the loaded embedding vectors, making them available for further processing or application within the image generation pipeline. Type should be `EMBEDS`.
