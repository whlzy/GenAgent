- `Image Generate Gradient`: This node is designed to generate images with gradient effects based on specified color stops, direction, and size. It allows for the creation of visually appealing backgrounds or elements by blending colors smoothly across the image in either a horizontal or vertical direction, with an option to adjust the tolerance for color transitions.
    - Parameters:
        - `width`: Specifies the width of the generated gradient image. It determines how wide the image will be. Type should be `INT`.
        - `height`: Specifies the height of the generated gradient image. It determines how tall the image will be. Type should be `INT`.
        - `direction`: Determines the direction of the gradient transition in the image, either horizontal or vertical. Type should be `COMBO[STRING]`.
        - `tolerance`: Adjusts the tolerance for color transitions in the gradient, affecting the smoothness of the gradient effect. Type should be `INT`.
        - `gradient_stops`: Defines the color stops for the gradient, specifying the colors and their positions within the gradient transition. Type should be `STRING`.
    - Inputs:
    - Outputs:
        - `image`: The generated image with the specified gradient effect. Type should be `IMAGE`.
