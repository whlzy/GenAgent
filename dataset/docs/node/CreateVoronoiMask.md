- `CreateVoronoiMask`: The CreateVoronoiMask node is designed to generate dynamic Voronoi diagram-based masks. It utilizes parameters such as the number of points, line width, and animation speed to create visually distinct and animated masks suitable for various creative and graphical applications.
    - Parameters:
        - `frames`: Specifies the number of frames for the animated mask, allowing for the creation of dynamic, time-varying masks. Type should be `INT`.
        - `num_points`: Determines the number of points used to generate the Voronoi diagram, affecting the complexity and appearance of the resulting mask. Type should be `INT`.
        - `line_width`: Sets the width of the lines in the Voronoi diagram, influencing the visual thickness of the mask's edges. Type should be `INT`.
        - `speed`: Controls the animation speed of the mask, enabling the adjustment of how quickly the mask evolves over time. Type should be `FLOAT`.
        - `frame_width`: Defines the width of the frame for the mask, setting the horizontal dimension of the generated mask. Type should be `INT`.
        - `frame_height`: Specifies the height of the frame for the mask, establishing the vertical dimension of the generated mask. Type should be `INT`.
    - Inputs:
    - Outputs:
        - `mask`: The generated Voronoi diagram-based mask. Type should be `MASK`.
        - `mask_inverted`: The inverted version of the generated Voronoi diagram-based mask, offering an alternative visual representation. Type should be `MASK`.
