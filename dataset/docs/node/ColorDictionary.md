- `ColorDictionary`: The ColorDictionary node provides a predefined set of color names and their corresponding RGB values. It allows for the selection of a specific number of colors from this set, based on the input parameter, to create a customized color dictionary.
    - Parameters:
        - `number_of_colors`: Specifies the number of colors to select from the predefined set. This determines the size of the resulting color dictionary. Type should be `INT`.
    - Inputs:
    - Outputs:
        - `color_dict`: A dictionary mapping color names to their RGB values, limited by the specified number of colors. Type should be `COLOR_DICT`.
