- `CR Repeater`: The CR Repeater node is designed to replicate items within a list or a single item multiple times based on a specified repeat count. It aims to facilitate the generation of extended datasets or the amplification of existing data elements for further processing.
    - Parameters:
        - `repeats`: Specifies the number of times the input data should be repeated. This parameter directly influences the size of the output list, allowing for controlled data expansion. Type should be `INT`.
    - Inputs:
        - `input_data`: Represents the data to be repeated. It can be a single item or a list of items, determining the scope of repetition within the node's operation. Type should be `*`.
    - Outputs:
        - `list`: A list containing the repeated instances of the input data, expanded according to the specified repeat count. Type should be `*`.
        - `show_help`: Provides a URL to the documentation or help page for the CR Repeater node, offering additional information and usage guidelines. Type should be `STRING`.
