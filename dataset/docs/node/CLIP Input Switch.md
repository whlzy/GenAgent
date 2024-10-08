- `CLIP Input Switch`: The WAS_CLIP_Input_Switch node is designed to toggle between two CLIP model inputs based on a boolean condition. It facilitates dynamic input selection within workflows that utilize CLIP models, enhancing flexibility in processing visual content.
    - Parameters:
        - `boolean`: A boolean condition that determines which CLIP model input (clip_a or clip_b) is selected for output. Type should be `BOOLEAN`.
    - Inputs:
        - `clip_a`: The first CLIP model input. Acts as the default selection when the boolean condition is true. Type should be `CLIP`.
        - `clip_b`: The second CLIP model input. It is selected when the boolean condition is false. Type should be `CLIP`.
    - Outputs:
        - `clip`: The selected CLIP model input based on the boolean condition. Type should be `CLIP`.
