- `LLMOpenAIModel`: This node facilitates the integration and utilization of OpenAI's language models, enabling the loading and embedding of models for various applications such as text generation, analysis, and more. It abstracts the complexity of directly interacting with OpenAI's API, providing a streamlined interface for embedding and model management.
    - Parameters:
        - `model`: Specifies the OpenAI model to be loaded. This selection determines the capabilities and performance of the language model in use. Type should be `COMBO[STRING]`.
        - `api_key`: The API key required for authenticating requests to OpenAI's services. It ensures secure access to the model loading functionality. Type should be `STRING`.
        - `embedding_model`: Defines the specific embedding model to be used alongside the primary language model, enhancing its functionality with additional text embedding capabilities. Type should be `COMBO[STRING]`.
        - `multimodal`: A boolean flag indicating whether the model to be loaded should support multimodal inputs, allowing for a broader range of input types beyond text. Type should be `BOOLEAN`.
    - Inputs:
    - Outputs:
        - `llm_model`: Returns the primary language model loaded, including its configuration and capabilities, ready for various applications. Type should be `LLM_MODEL`.
        - `embed_model_only`: Provides the embedding model loaded separately, detailing its specific features and how it complements the primary language model. Type should be `LLM_EMBED_MODEL`.
