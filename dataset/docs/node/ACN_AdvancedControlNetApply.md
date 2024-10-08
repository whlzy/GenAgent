- `ACN_AdvancedControlNetApply`: This node applies advanced control networks to modify the conditioning of an image based on specified control nets, images, and strength parameters. It enables the dynamic adjustment of image attributes through control networks, enhancing the flexibility and precision of image conditioning.
    - Parameters:
        - `strength`: Determines the intensity of the control net's effect on the image conditioning. A higher value results in more pronounced modifications. Type should be `FLOAT`.
        - `start_percent`: Defines the starting percentage of the effect applied by the control net, allowing for gradual application of the control net's effect over the image. Type should be `FLOAT`.
        - `end_percent`: Defines the ending percentage of the effect applied by the control net, enabling precise control over how the effect tapers off. Type should be `FLOAT`.
    - Inputs:
        - `positive`: Specifies the positive conditioning data that the control net will modify, contributing to the enhancement of desired image attributes. Type should be `CONDITIONING`.
        - `negative`: Specifies the negative conditioning data that the control net will adjust, aiming to suppress undesired image attributes. Type should be `CONDITIONING`.
        - `control_net`: The control net to be applied. It defines the specific modifications and adjustments to be made to the conditioning, directly influencing the outcome. Type should be `CONTROL_NET`.
        - `image`: The image to which the control net adjustments will be applied. It serves as the visual content that will be modified according to the control net's specifications. Type should be `IMAGE`.
        - `mask_optional`: An optional mask that can be applied to target specific areas of the image for conditioning adjustments. Type should be `MASK`.
        - `timestep_kf`: Optional keyframe for specifying the timestep at which the control net's effect should be applied, allowing for temporal control. Type should be `TIMESTEP_KEYFRAME`.
        - `latent_kf_override`: Allows for overriding the latent keyframes, providing flexibility in how the control net's effects are applied over time. Type should be `LATENT_KEYFRAME`.
        - `weights_override`: Optional parameter to override the default weights of the control net, offering customization of the control net's influence. Type should be `CONTROL_NET_WEIGHTS`.
        - `model_optional`: An optional model parameter that, if provided, will be used instead of the default control net model, allowing for further customization. Type should be `MODEL`.
    - Outputs:
        - `positive`: The modified positive conditioning data after applying the control net, reflecting the enhancements made. Type should be `CONDITIONING`.
        - `negative`: The modified negative conditioning data after applying the control net, reflecting the suppression of undesired attributes. Type should be `CONDITIONING`.
        - `model_opt`: An optional output model that may be modified by the node's processing, available for further use. Type should be `MODEL`.
