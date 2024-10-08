- `LLMHtmlRepair`: The LLMHtmlRepair node leverages a language model to analyze and correct malformed HTML content, ensuring the output is well-structured and valid HTML without data loss.
    - Parameters:
        - `text_input`: The malformed HTML content that needs to be repaired. It serves as the primary input for the correction process. Type should be `STRING`.
        - `extra_directions`: Optional additional instructions for the language model, guiding the repair process with more specificity. Type should be `STRING`.
    - Inputs:
        - `llm_model`: Specifies the language model to use for repairing the HTML. It's crucial for interpreting the input and generating the corrected HTML. Type should be `LLM_MODEL`.
    - Outputs:
        - `html_output`: The repaired HTML content, which is well-structured and valid, ensuring no data is omitted. Type should be `STRING`.
