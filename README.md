# Text2Video-CogVideoX

## Introduction

Text2Video-CogVideoX is a project that leverages the CogVideo model to generate videos from text prompts. This repository contains the necessary scripts and notebooks to set up the model, generate videos, and perform related tasks.

## Installation

To get started, clone this repository and install the required dependencies:

```bash
git clone https://github.com/aayush1693/Text2Video-CogVideoX
cd Text2Video-CogVideoX
pip install -r requirements.txt
```

## Usage

### Running the Notebook

You can use the `CogVideoX_2b.ipynb` notebook to generate videos from text prompts. Follow these steps:

1. Open the notebook:
    ```bash
    jupyter notebook CogVideoX_2b.ipynb
    ```

2. Follow the steps in the notebook to set up the environment, install dependencies, and generate videos.

### Running the Script

You can also use the `cogvideox_2b.py` script to generate videos:

1. Modify the script to include your text prompt:
    ```python
    prompt = "A beautiful waterfall in a forest"
    ```

2. Run the script:
    ```bash
    python cogvideox_2b.py
    ```

## Model Explanation

### CogVideo Model

CogVideo is a generative model designed to create videos from text descriptions. It uses a transformer-based architecture to interpret text prompts and generate corresponding video frames. The model is trained on extensive datasets to understand the relationship between textual descriptions and visual representations.

#### Key Features

- **Transformer Architecture**: Utilizes a transformer model for both text encoding and video frame generation.
- **Quantization**: The model is quantized to reduce memory usage and improve efficiency.
- **GPU Acceleration**: Leverages GPU for faster video generation.

### Theory Behind CogVideo

The CogVideo model operates by encoding a text prompt into a latent representation, which is then used to generate video frames. The process involves several steps:

1. **Text Encoding**: The text prompt is encoded into a latent vector using a transformer encoder.
2. **Frame Generation**: The latent vector is fed into a decoder that generates individual video frames.
3. **Optimization**: Techniques like quantization and mixed-precision training are used to optimize memory usage and computation.

The model iteratively generates video frames, ensuring that each frame is coherent with the preceding ones, thus creating a smooth video sequence.

## Acknowledgments

This project utilizes the CogVideo model developed by the [THUDM](https://github.com/THUDM/CogVideo) team. We extend our sincere thanks to the inventors of CogVideo for their groundbreaking work in the field of video generation.

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for more details.

## Contributing

We welcome contributions from the community. If you have any ideas or improvements, please feel free to open a pull request or issue.

## Contact

For any questions or inquiries, please contact [Aayush Parajuli](mailto:parajuliaayush@gmail.com).


