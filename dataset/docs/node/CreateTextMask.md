- `CreateTextMask`: The CreateTextMask node is designed to generate a text-based image and its corresponding mask, utilizing a variety of fonts and supporting animation through rotation parameters. It enables the creation of dynamic text visuals for various applications.
    - Parameters:
        - `invert`: Determines whether the colors of the generated text image and mask should be inverted, affecting the visual contrast and style. Type should be `BOOLEAN`.
        - `frames`: Specifies the number of frames to generate, allowing for the creation of animated sequences if more than one frame is used. Type should be `INT`.
        - `text_x`: Sets the horizontal position of the text within the image, enabling precise placement. Type should be `INT`.
        - `text_y`: Sets the vertical position of the text within the image, allowing for vertical alignment adjustments. Type should be `INT`.
        - `font_size`: Controls the size of the font used for the text, impacting the readability and visual impact of the text. Type should be `INT`.
        - `font_color`: Defines the color of the text, offering customization options for the text's appearance. Type should be `STRING`.
        - `text`: The text content to be rendered in the image, serving as the primary visual element. Type should be `STRING`.
        - `font`: Selects the font to be used for the text, providing a range of stylistic choices. The font list is dynamically generated based on available fonts in a specified directory. Type should be `COMBO[STRING]`.
        - `width`: Determines the width of the generated image, defining the canvas size. Type should be `INT`.
        - `height`: Determines the height of the generated image, defining the canvas size. Type should be `INT`.
        - `start_rotation`: Sets the starting rotation angle for the text, enabling rotational animation effects when combined with end_rotation. Type should be `INT`.
        - `end_rotation`: Sets the ending rotation angle for the text, enabling the creation of rotational animation effects. Type should be `INT`.
    - Inputs:
    - Outputs:
        - `image`: The text-based image generated by the node, which can be used directly or further processed. Type should be `IMAGE`.
        - `mask`: The mask generated alongside the text image, useful for further image processing or effects. Type should be `MASK`.
