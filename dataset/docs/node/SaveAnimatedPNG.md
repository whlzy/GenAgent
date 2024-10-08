- `SaveAnimatedPNG`: The SaveAnimatedPNG node is designed for creating and saving animated PNG images from a sequence of frames. It handles the assembly of individual image frames into a cohesive animation, allowing for customization of frame duration, looping, and metadata inclusion.
    - Parameters:
        - `filename_prefix`: Specifies the base name for the output file, which will be used as a prefix for the generated animated PNG files. Type should be `STRING`.
        - `fps`: The frames per second rate for the animation, controlling how quickly the frames are displayed. Type should be `FLOAT`.
        - `compress_level`: The level of compression applied to the animated PNG files, affecting file size and image clarity. Type should be `INT`.
    - Inputs:
        - `images`: A list of images to be processed and saved as an animated PNG. Each image in the list represents a frame in the animation. Type should be `IMAGE`.
    - Outputs:
