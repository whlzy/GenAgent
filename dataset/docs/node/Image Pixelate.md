- `Image Pixelate`: The node is designed to transform images into pixel art by applying pixelation, color reduction, and optionally dithering. It supports customization of pixelation size, number of colors, initial color selection mode, dithering options, and color palettes, allowing for a wide range of artistic effects.
    - Parameters:
        - `pixelation_size`: Specifies the size of the pixels in the resulting pixel art, controlling the level of detail and abstraction. Type should be `FLOAT`.
        - `num_colors`: Determines the number of colors used in the pixel art, affecting the color complexity and style. Type should be `FLOAT`.
        - `init_mode`: Defines the initial color selection mode, influencing the starting point for color optimization. Type should be `COMBO[STRING]`.
        - `max_iterations`: Sets the maximum number of iterations for color optimization, impacting the refinement of the final pixel art. Type should be `FLOAT`.
        - `dither`: Enables or disables dithering, a technique to simulate additional colors and gradients through patterns. Type should be `COMBO[STRING]`.
        - `dither_mode`: Selects the dithering algorithm to be used, influencing the pattern and appearance of simulated colors. Type should be `COMBO[STRING]`.
        - `color_palette_mode`: Determines how the color palettes are applied, affecting the gradient and transition between colors. Type should be `COMBO[STRING]`.
        - `reverse_palette`: When enabled, reverses the order of colors in the palette, allowing for different visual effects. Type should be `COMBO[STRING]`.
    - Inputs:
        - `images`: The images to be transformed into pixel art. This input is crucial for defining the base content that will undergo pixelation and color reduction. Type should be `IMAGE`.
        - `color_palettes`: A list of color palettes to be used for coloring the pixel art, offering additional customization for the final appearance. Type should be `LIST`.
    - Outputs:
        - `images`: The resulting pixel art images, transformed from the original inputs through pixelation, color reduction, and optional dithering. Type should be `IMAGE`.
