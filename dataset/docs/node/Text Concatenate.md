- `Text Concatenate`: The Text Concatenate node is designed to merge multiple text inputs into a single string, using a specified delimiter. It offers the option to clean up whitespace, ensuring that the concatenated result is tidy and adheres to the desired formatting.
    - Parameters:
        - `delimiter`: Specifies the character or string used to separate each text input in the concatenated result. It plays a crucial role in defining the structure and readability of the output. Type should be `STRING`.
        - `clean_whitespace`: Determines whether leading and trailing whitespace should be removed from each text input before concatenation, ensuring a clean and consistent output format. This parameter should be provided as a boolean value. Type should be `COMBO[STRING]`.
        - `text_a`: Accepts a text input as a string. This input is one of the strings to be concatenated, allowing for dynamic and flexible text merging. Type should be `STRING`.
        - `text_b`: Accepts a text input as a string. This input is one of the strings to be concatenated, allowing for dynamic and flexible text merging. Type should be `STRING`.
        - `text_c`: Accepts a text input as a string. This input is one of the strings to be concatenated, allowing for dynamic and flexible text merging. Type should be `STRING`.
        - `text_d`: Accepts a text input as a string. This input is one of the strings to be concatenated, allowing for dynamic and flexible text merging. Type should be `STRING`.
    - Inputs:
    - Outputs:
        - `string`: The final string resulting from the concatenation of all provided text inputs, formatted according to the specified delimiter and whitespace cleaning settings. Type should be `STRING`.
