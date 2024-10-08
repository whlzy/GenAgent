- `Number Input Switch`: The Number Input Switch node provides a mechanism to select between two numerical inputs based on a boolean condition. It is designed to facilitate conditional logic within data flows, allowing for dynamic selection of input values.
    - Parameters:
        - `boolean`: A boolean flag that determines which of the two numerical inputs (number_a or number_b) is selected for output. Type should be `BOOLEAN`.
    - Inputs:
        - `number_a`: Represents the first numerical input option for the switch. Its value is considered if the boolean condition is true. Type should be `NUMBER`.
        - `number_b`: Represents the second numerical input option for the switch. Its value is considered if the boolean condition is false. Type should be `NUMBER`.
    - Outputs:
        - `number`: The original number selected based on the boolean condition. Type should be `NUMBER`.
        - `float`: The float representation of the selected number. Type should be `FLOAT`.
        - `int`: The integer representation of the selected number. Type should be `INT`.
