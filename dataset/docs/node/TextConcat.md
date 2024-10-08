- `TextConcat`: The TextConcat node is designed to merge multiple text inputs into a single string, offering the flexibility to specify a delimiter for the concatenation. This functionality is particularly useful for combining pieces of text in a customizable manner.
    - Parameters:
        - `delimiter`: Specifies the character or string used to separate the concatenated texts. Its presence allows for customizable spacing or formatting between the merged text inputs. Type should be `STRING`.
        - `text1`: Represents the first optional text input to be concatenated. If provided, it contributes to the final merged string. Type should be `STRING`.
        - `text2`: Represents the second optional text input to be concatenated. If provided, it contributes to the final merged string. Type should be `STRING`.
        - `text3`: Represents the third optional text input to be concatenated. If provided, it contributes to the final merged string. Type should be `STRING`.
        - `text4`: Represents the fourth optional text input to be concatenated. If provided, it contributes to the final merged string. Type should be `STRING`.
        - `text5`: Represents the fifth optional text input to be concatenated. If provided, it contributes to the final merged string. Type should be `STRING`.
    - Inputs:
    - Outputs:
        - `string`: The output is a single string that results from the concatenation of the provided text inputs, separated by the specified delimiter. Type should be `STRING`.
