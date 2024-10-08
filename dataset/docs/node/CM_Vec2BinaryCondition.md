- `CM_Vec2BinaryCondition`: This node performs a binary condition operation between two 2-dimensional vectors, evaluating to a boolean result based on the specified operation.
    - Parameters:
        - `op`: Specifies the binary condition operation to be applied between the two vectors, determining the nature of the comparison. Type should be `COMBO[STRING]`.
    - Inputs:
        - `a`: The first 2-dimensional vector involved in the binary condition operation. Type should be `VEC2`.
        - `b`: The second 2-dimensional vector involved in the binary condition operation. Type should be `VEC2`.
    - Outputs:
        - `bool`: The boolean result of the binary condition operation between the two vectors. Type should be `BOOL`.
