# mark2.2.0
- Influenced by mark2.1.2 but changed more efficiently
- Although based on mark2.1.2, two new scripts were added: segments.py and fix_audio_length_to_240000.py.
- During training, analysis using segments.py revealed that the number of segments in audio files is not always perfectly consistent.
- To address this, fix_audio_length_to_240000.py was introduced to ensure consistency in the number of segments for future training. This script trims audio files longer than 15.00 seconds and applies zero-padding to slightly shorter ones. It also resamples all audio to a fixed sample rate of 16,000 Hz to maintain consistent frequency resolution.

## License
- This project is licensed under the PolyForm Noncommercial License 1.0.0.
- Commercial use is not permitted.
- See the [LICENSE](LICENSE) file for details.
