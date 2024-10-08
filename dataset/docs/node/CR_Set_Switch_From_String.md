- `CR Set Switch From String`: This node dynamically sets a switch based on a string input, allowing for conditional logic flows within a node network. It supports up to four predefined string conditions to determine the switch's state.
    - Parameters:
        - `text`: The primary string input used to determine the switch's state. It's essential for executing the node's logic and determining the output. Type should be `STRING`.
        - `switch_1`: A predefined condition string. If it matches the 'text' input, the switch is set to 1. Type should be `STRING`.
        - `switch_2`: A predefined condition string. If it matches the 'text' input, the switch is set to 2. Type should be `STRING`.
        - `switch_3`: A predefined condition string. If it matches the 'text' input, the switch is set to 3. Type should be `STRING`.
        - `switch_4`: A predefined condition string. If it matches the 'text' input, the switch is set to 4. Type should be `STRING`.
    - Inputs:
    - Outputs:
        - `switch`: The output switch state determined by the input string, indicating which condition was met. Type should be `INT`.
        - `show_help`: A URL providing additional help and documentation for using this node. Type should be `STRING`.
