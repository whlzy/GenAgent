- `StringFunctionpysssss`: The String Function node provides utilities for manipulating strings, including appending, replacing, and optionally tidying tags within given text inputs. It abstracts complex string operations into a simple interface, catering to a variety of text processing needs.
    - Parameters:
        - `action`: Specifies the string manipulation action to perform, such as appending or replacing content in the text inputs. Type should be `COMBO[STRING]`.
        - `tidy_tags`: Determines whether to clean up HTML tags in the text inputs, offering options to either tidy them or leave them as is. Type should be `COMBO[STRING]`.
        - `text_a`: The primary text input for manipulation. Type should be `STRING`.
        - `text_b`: The secondary text input for manipulation, used in conjunction with 'text_a'. Type should be `STRING`.
        - `text_c`: An optional third text input for manipulation. Type should be `STRING`.
    - Inputs:
    - Outputs:
        - `string`: The result of the string manipulation, returned as a single string. Type should be `STRING`.
