- `SaltAudioMixer`: The SaltAudioMixer node is designed to blend two audio inputs into a single output by overlaying one audio segment onto another at a specified mix time. This functionality is essential for creating composite audio tracks from multiple sources, allowing for dynamic audio mixing in multimedia projects.
    - Parameters:
        - `mix_time_seconds`: Specifies the time offset in seconds at which the second audio input (audio_b) will be overlaid onto the first (audio_a). This parameter allows for precise control over the timing of the audio mix. Type should be `FLOAT`.
    - Inputs:
        - `audio_a`: The first audio input to be mixed. It serves as the base layer onto which the second audio input will be overlaid. Type should be `AUDIO`.
        - `audio_b`: The second audio input to be mixed. This audio is overlaid onto the first input at the specified mix time, contributing to the composite output. Type should be `AUDIO`.
    - Outputs:
        - `mixed_audio`: The resulting audio after mixing the two inputs. This output is a single audio track that combines elements of both input tracks. Type should be `AUDIO`.
