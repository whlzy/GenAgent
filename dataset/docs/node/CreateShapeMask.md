- `CreateShapeMask`: The CreateShapeMask node is designed for generating masks or batches of masks with specific shapes. It allows for dynamic creation of animated masks by adjusting the growth of the shape across frames, providing a versatile tool for mask generation in various dimensions and shapes.
    - Parameters:
        - `shape`: Specifies the geometric shape of the mask to be created. This choice influences the visual appearance and boundary of the generated mask. Type should be `COMBO[STRING]`.
        - `frames`: Determines the number of frames for the animated mask, allowing for the creation of a sequence of masks with progressive growth. Type should be `INT`.
        - `location_x`: The x-coordinate for the center location of the shape, defining where the shape will be positioned horizontally within the frame. Type should be `INT`.
        - `location_y`: The y-coordinate for the center location of the shape, defining where the shape will be positioned vertically within the frame. Type should be `INT`.
        - `grow`: Controls the amount by which the shape grows on each frame, enabling the animation of the mask. Type should be `INT`.
        - `frame_width`: The width of the frame in which the shape is placed, setting the horizontal boundary for the mask. Type should be `INT`.
        - `frame_height`: The height of the frame in which the shape is placed, setting the vertical boundary for the mask. Type should be `INT`.
        - `shape_width`: Specifies the initial width of the shape, determining its size before any growth is applied. Type should be `INT`.
        - `shape_height`: Specifies the initial height of the shape, determining its size before any growth is applied. Type should be `INT`.
    - Inputs:
    - Outputs:
        - `mask`: The generated mask with the specified shape and dimensions. Type should be `MASK`.
        - `mask_inverted`: An inverted version of the generated mask, where the shape's area is transparent and the rest is opaque. Type should be `MASK`.
