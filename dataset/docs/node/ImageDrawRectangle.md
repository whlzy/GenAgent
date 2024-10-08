- `ImageDrawRectangle`: The `ImageDrawRectangle` node provides functionality for drawing rectangles on images. It allows for the customization of the rectangle's dimensions, outline, and fill properties, enabling users to add simple geometric shapes to their images for various purposes such as highlighting areas, creating borders, or adding visual annotations.
    - Parameters:
        - `width`: Specifies the width of the canvas on which the rectangle will be drawn, affecting the overall dimensions of the image. Type should be `INT`.
        - `height`: Specifies the height of the canvas on which the rectangle will be drawn, affecting the overall dimensions of the image. Type should be `INT`.
        - `start_x`: Specifies the starting x-coordinate of the rectangle, influencing the horizontal position where the rectangle drawing begins. Type should be `FLOAT`.
        - `start_y`: Specifies the starting y-coordinate of the rectangle, affecting the vertical position where the rectangle drawing begins. Type should be `FLOAT`.
        - `end_x`: Specifies the ending x-coordinate of the rectangle, determining the horizontal extent of the rectangle. Type should be `FLOAT`.
        - `end_y`: Specifies the ending y-coordinate of the rectangle, determining the vertical extent of the rectangle. Type should be `FLOAT`.
        - `outline_size`: Determines the thickness of the rectangle's outline, allowing for customization of the rectangle's border appearance. Type should be `INT`.
        - `outline_red`: Specifies the red component of the outline's color, contributing to the overall color of the rectangle's border. Type should be `INT`.
        - `outline_green`: Specifies the green component of the outline's color, contributing to the overall color of the rectangle's border. Type should be `INT`.
        - `outline_blue`: Specifies the blue component of the outline's color, contributing to the overall color of the rectangle's border. Type should be `INT`.
        - `outline_alpha`: Specifies the alpha (transparency) component of the outline's color, allowing for control over the opacity of the rectangle's border. Type should be `FLOAT`.
        - `fill_red`: Specifies the red component of the fill color, contributing to the overall color inside the rectangle. Type should be `INT`.
        - `fill_green`: Specifies the green component of the fill color, contributing to the overall color inside the rectangle. Type should be `INT`.
        - `fill_blue`: Specifies the blue component of the fill color, contributing to the overall color inside the rectangle. Type should be `INT`.
        - `fill_alpha`: Specifies the alpha (transparency) component of the fill color, allowing for control over the opacity of the color inside the rectangle. Type should be `FLOAT`.
        - `SSAA`: Super Sample Anti-Aliasing factor, which enhances the image quality by reducing the aliasing effects. Type should be `INT`.
        - `method`: The method parameter specifies the resizing algorithm used when adjusting the image's size, affecting the quality of the final output. Type should be `COMBO[STRING]`.
    - Inputs:
    - Outputs:
        - `image`: The output is an image tensor with the drawn rectangle, reflecting the modifications made to the original image. Type should be `IMAGE`.
