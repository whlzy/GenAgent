- `Mask To Region`: The 'Mask To Region' node is designed to transform a given mask into a rectangular region that encompasses the mask, adhering to specified constraints such as padding, aspect ratio, and minimum dimensions. This node facilitates the extraction of meaningful regions from masks for further processing or analysis.
    - Parameters:
        - `padding`: The 'padding' parameter allows specifying additional space around the identified region, enhancing flexibility in region extraction. Type should be `INT`.
        - `constraints`: The 'constraints' parameter defines the rules for adjusting the extracted region's dimensions, including keeping aspect ratios and size multiples. Type should be `COMBO[STRING]`.
        - `constraint_x`: The 'constraint_x' parameter sets a constraint on the region's width, ensuring it adheres to specified requirements. Type should be `INT`.
        - `constraint_y`: The 'constraint_y' parameter sets a constraint on the region's height, ensuring it adheres to specified requirements. Type should be `INT`.
        - `min_width`: The 'min_width' parameter establishes a minimum width for the extracted region, ensuring it meets a certain size threshold. Type should be `INT`.
        - `min_height`: The 'min_height' parameter establishes a minimum height for the extracted region, ensuring it meets a certain size threshold. Type should be `INT`.
        - `batch_behavior`: The 'batch_behavior' parameter dictates how the node should handle multiple masks in a batch, focusing on matching aspect ratios or sizes. Type should be `COMBO[STRING]`.
    - Inputs:
        - `mask`: The 'mask' parameter represents the input mask image that the node will process to identify and extract the rectangular region. Type should be `IMAGE`.
    - Outputs:
        - `image`: The output is an image of the rectangular region extracted from the input mask, conforming to the specified constraints. Type should be `IMAGE`.
