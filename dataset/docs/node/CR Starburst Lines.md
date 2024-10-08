- `CR Starburst Lines`: This node is designed to generate a starburst pattern with lines radiating from a central point. It allows customization of various aspects such as the number of lines, their length, color, and rotation, enabling the creation of visually striking graphics.
    - Parameters:
        - `width`: Specifies the width of the canvas for the starburst pattern. Type should be `INT`.
        - `height`: Specifies the height of the canvas for the starburst pattern. Type should be `INT`.
        - `num_lines`: Specifies the number of lines in the starburst pattern. This determines how densely the lines are packed together, affecting the overall appearance of the starburst. Type should be `INT`.
        - `line_length`: Defines the length of each line in the starburst pattern. Longer lines will extend further from the center, creating a more pronounced effect. Type should be `FLOAT`.
        - `line_width`: Sets the width of the lines in the starburst pattern. Thicker lines will make the starburst more visible and pronounced. Type should be `INT`.
        - `line_color`: Determines the color of the lines in the starburst pattern. This can be a predefined color or a custom hex value, allowing for extensive customization. Type should be `COMBO[STRING]`.
        - `background_color`: Determines the background color of the canvas. This can be a predefined color or 'custom' to use a hex value specified in 'bg_color_hex'. Type should be `COMBO[STRING]`.
        - `center_x`: Specifies the x-coordinate of the center point from which the starburst lines radiate. Type should be `INT`.
        - `center_y`: Specifies the y-coordinate of the center point from which the starburst lines radiate. Type should be `INT`.
        - `rotation`: Specifies the rotation angle of the entire starburst pattern. This allows the pattern to be oriented in any direction. Type should be `FLOAT`.
        - `line_color_hex`: Specifies the custom hex color value for the lines if 'line_color' is set to 'custom'. Type should be `STRING`.
        - `bg_color_hex`: Specifies the custom hex color value for the background if 'background_color' is set to 'custom'. Type should be `STRING`.
    - Inputs:
    - Outputs:
        - `IMAGE`: The generated image featuring the starburst pattern. Type should be `IMAGE`.
        - `show_help`: A URL to documentation or help page related to the starburst pattern generation. Type should be `STRING`.
