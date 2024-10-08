- `ADE_StandardUniformContextOptions`: This node is designed to create a uniform set of context options for animation difference processing, allowing for the customization of context length, start percentage, and guaranteed steps within the animation sequence. It supports the integration of previous context configurations to build upon existing settings.
    - Parameters:
        - `context_length`: Specifies the length of the context for the animation difference processing, influencing the granularity and scope of the animation sequence. Type should be `INT`.
        - `context_stride`: Determines the stride between each context in the sequence, affecting the overlap and transition smoothness between animation frames. Type should be `INT`.
        - `context_overlap`: Defines the amount of overlap between contexts, which can influence the continuity and smoothness of the animation. Type should be `INT`.
        - `fuse_method`: Specifies the method used to fuse multiple contexts together, impacting the final animation's visual coherence. Type should be `COMBO[STRING]`.
        - `use_on_equal_length`: Indicates whether the context options should be applied uniformly across animations of equal length, affecting consistency in animation processing. Type should be `BOOLEAN`.
        - `start_percent`: Determines the starting point of the animation as a percentage, allowing for precise control over the initiation of the animation sequence. Type should be `FLOAT`.
        - `guarantee_steps`: Defines the minimum number of steps guaranteed within the animation, ensuring a certain level of detail and smoothness in the animation sequence. Type should be `INT`.
    - Inputs:
        - `prev_context`: Allows for the inclusion of previous context configurations, enabling the accumulation and refinement of context settings over time. Type should be `CONTEXT_OPTIONS`.
        - `view_opts`: Allows for the specification of view options, further customizing the context configuration for animation processing. Type should be `VIEW_OPTS`.
    - Outputs:
        - `CONTEXT_OPTS`: Produces a set of context options tailored for uniform animation difference processing, encapsulating the specified configurations. Type should be `CONTEXT_OPTIONS`.
