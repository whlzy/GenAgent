- `CR Cycle Images Simple`: This node is designed to cycle through a simple list of images in a sequential manner, based on the current frame and a specified frame interval. It allows for the creation of simple animations by iterating over a collection of images a specified number of times (loops).
    - Parameters:
        - `mode`: Specifies the cycling mode, which determines how images are cycled through. For this node, 'Sequential' mode is used to cycle images in order. Type should be `COMBO[STRING]`.
        - `frame_interval`: Defines the number of frames to wait before transitioning to the next image in the sequence, allowing control over the animation speed. Type should be `INT`.
        - `loops`: Determines how many times the list of images will be cycled through, enabling repeated animations. Type should be `INT`.
        - `current_frame`: Indicates the current frame number in the animation sequence, used to calculate which image to display. Type should be `INT`.
    - Inputs:
        - `image_1`: The first image in the sequence to be cycled through. Type should be `IMAGE`.
        - `image_2`: The second image in the sequence to be cycled through. Type should be `IMAGE`.
        - `image_3`: The third image in the sequence to be cycled through. Type should be `IMAGE`.
        - `image_4`: The fourth image in the sequence to be cycled through. Type should be `IMAGE`.
        - `image_5`: The fifth image in the sequence to be cycled through. Type should be `IMAGE`.
        - `image_list_simple`: An optional list of images to be cycled through, providing an alternative or additional set of images for the animation. Type should be `IMAGE_LIST_SIMPLE`.
    - Outputs:
        - `IMAGE`: The image to be displayed at the current frame of the animation. Type should be `IMAGE`.
        - `show_help`: A URL providing additional help and information about the node. Type should be `STRING`.
