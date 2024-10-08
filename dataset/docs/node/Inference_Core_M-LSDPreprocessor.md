- `Inference_Core_M-LSDPreprocessor`: The M-LSD Preprocessor node is designed for extracting line segments from images using the M-LSD (Multi-Level Line Segment Detector) model. It processes images to detect and delineate line structures, facilitating tasks that require understanding of geometric shapes and structures within the visual data.
    - Parameters:
        - `score_threshold`: Defines the confidence threshold for line segment detection. Lines with scores below this threshold are discarded, influencing the sensitivity of the detection process. Type should be `FLOAT`.
        - `dist_threshold`: Sets the distance threshold for separating line segments. This parameter helps in distinguishing between closely spaced lines, affecting the granularity of the detected lines. Type should be `FLOAT`.
        - `resolution`: Specifies the resolution at which the image is processed. This affects the scale of detection and can influence the detection of line segments. Type should be `INT`.
    - Inputs:
        - `image`: The input image to be processed for line segment detection. It serves as the primary data on which the M-LSD model operates. Type should be `IMAGE`.
    - Outputs:
        - `image`: The output is an image annotated with detected line segments, visually representing the geometric structures identified by the M-LSD model. Type should be `IMAGE`.
