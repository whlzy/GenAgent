- `CLIPEncodeMultipleAdvanced`: This node is designed for advanced text encoding using the CLIP model, allowing for the customization of token normalization and weight interpretation. It supports encoding multiple inputs simultaneously, adjusting the encoding process based on the provided parameters to generate a list of conditionings.
    - Parameters:
        - `token_normalization`: Determines whether or not to normalize tokens during the encoding process, affecting the final embeddings. Type should be `COMBO[STRING]`.
        - `weight_interpretation`: Adjusts the weight interpretation for the encoding, influencing how the embeddings are calculated. Type should be `COMBO[STRING]`.
        - `inputs_len`: Specifies the number of inputs to encode. This allows the node to handle multiple inputs simultaneously, generating a list of conditionings. Type should be `INT`.
    - Inputs:
        - `clip`: The CLIP model used for encoding. It's crucial for interpreting the input text into embeddings. Type should be `CLIP`.
    - Outputs:
        - `conditioning`: Generates a list of conditionings based on the encoded inputs. This is crucial for subsequent processing steps that rely on these conditionings. Type should be `CONDITIONING`.
