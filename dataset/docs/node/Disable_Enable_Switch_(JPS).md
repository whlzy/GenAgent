- `Disable Enable Switch (JPS)`: This node toggles between disabling and enabling a feature based on the comparison of two integer values and a match condition.
    - Parameters:
        - `select`: Specifies the first integer value to be compared, influencing the switch's outcome. Type should be `INT`.
        - `compare`: Specifies the second integer value to be compared against the first, affecting the switch's result. Type should be `INT`.
        - `match`: Determines the condition ('Set to Disable' or 'Set to Enable') that controls the switch's behavior. Type should be `COMBO[STRING]`.
    - Inputs:
    - Outputs:
        - `disable_enable`: Outputs either 'disable' or 'enable' based on the comparison of input values and the match condition. Type should be `COMBO[STRING]`.
