- `VHS_LoadAudio`: The VHS_LoadAudio node is designed for loading audio files into the Video Helper Suite environment. It supports a variety of audio formats and allows for seeking a specific start time within the audio file, making it a versatile tool for audio processing and manipulation within video projects.
    - Parameters:
        - `audio_file`: Specifies the path to the audio file to be loaded. The node supports a range of audio formats, making it flexible for use with various audio sources. Type should be `STRING`.
        - `seek_seconds`: Determines the start time in seconds from which the audio should begin playing. This allows for precise control over the playback start time within the audio file. Type should be `FLOAT`.
    - Inputs:
    - Outputs:
        - `audio`: The loaded audio data, ready for use within the Video Helper Suite for further processing or integration into video projects. Type should be `VHS_AUDIO`.
