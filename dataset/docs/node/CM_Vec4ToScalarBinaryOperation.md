- `CM_Vec4ToScalarBinaryOperation`: This node performs a binary operation between two Vec4 vectors, resulting in a scalar value. It supports operations like dot product and distance calculation, transforming vector relationships into a single numerical outcome.
    - Parameters:
        - `op`: Specifies the binary operation to be performed, such as dot product or distance, affecting the scalar result. Type should be `COMBO[STRING]`.
    - Inputs:
        - `a`: The first Vec4 vector operand in the binary operation. Type should be `VEC4`.
        - `b`: The second Vec4 vector operand in the binary operation. Type should be `VEC4`.
    - Outputs:
        - `float`: The scalar result of the binary operation between the two Vec4 vectors. Type should be `FLOAT`.
