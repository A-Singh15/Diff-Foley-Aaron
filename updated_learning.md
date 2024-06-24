# Diff-Foley: Synchronized Video-to-Audio Synthesis with Latent Diffusion Models

## Key Components

### Key Components of CAVP

- **Video Encoder**: Extracts features from video frames.
- **Audio Encoder**: Extracts features from audio data.
- **Fusion Layer**: Combines the video and audio features.
- **Output Layer**: Generates the audio features or predictions.

### Key Components of LDM

- **Latent Encoder**: Encodes the input into a latent representation.
- **Latent Diffusion Process**: Refines the latent representation.
- **Latent Decoder**: Decodes the refined latent representation back into the audio domain.

## Differences Between CAVP and LDM

### Purpose

- **CAVP**: Focuses on learning the basic relationship between video and audio features.
- **LDM**: Refines the pretrained model to generate higher-quality audio using latent space and diffusion processes.

### Model Architecture

- **CAVP**: Typically involves direct encoding of video and audio features and a simple fusion mechanism.
- **LDM**: Involves more complex processes in the latent space, including the application of diffusion models to improve audio quality.

### Training Process

- **CAVP**: Trains on raw video and audio data to learn initial mappings.
- **LDM**: Uses the pretrained CAVP model and further trains it using latent representations and diffusion techniques to enhance performance.
