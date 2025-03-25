# Recurrent Neural Networks (RNNs) and LSTMs for Text Generation

This project demonstrates how to build a text generation model using Recurrent Neural Networks (RNNs) with Long Short-Term Memory (LSTM) layers in TensorFlow/Keras. We use a unique dataset, *Ancient Myths: A Collection of Global Legends*, which contains global myths and legends. This tutorial is designed as a step-by-step guide that is accessible and self-contained.

## Project Overview

- **Tutorial Focus:** 
  - Introduction to sequence models for text generation.
  - Explanation of RNNs, LSTMs, and GRUs.
  - Building and training an LSTM model in TensorFlow/Keras.
  - Experimenting with network depth to observe effects on text coherence.
- **Key Features:**
  - Detailed explanations of underlying techniques.
  - Well-commented code with accessibility considerations (color-friendly plots, clear visualizations).
  - A unique dataset for text generation.
- **Repository Contents:**
  - A Jupyter Notebook (`main.ipynb`) containing the full tutorial and code.
  - This README file.
  - MIT License (`LICENSE`).
  - Optional `requirements.txt` file listing required packages.

## How to Run the Project

### 1. Clone the Repository

Clone the repository to your local machine using Git:

```bash
git clone https://github.com/UmerCheena/RNNs-and-LSTMs-for-Text-Generation.git
cd RNNs-and-LSTMs-for-Text-Generation
```

### 2. Set Up the Environment

It is recommended to use a virtual environment to manage dependencies. Make sure you have Python 3.x installed.

```bash
# Create and activate a virtual environment
python3 -m venv venv
source venv/bin/activate  # For Windows: venv\Scripts\activate

# Install required packages
pip install -r requirements.txt
```

*Note: If a `requirements.txt` file is not provided, create one with the following content:*

```text
tensorflow
numpy
matplotlib
```

### 3. Run the Jupyter Notebook

Launch the Jupyter Notebook to view and run the tutorial code:

```bash
jupyter main.ipynb
```

Follow the notebook's instructions to learn about data preprocessing, building the model, training, text generation, and evaluating model performance.

## Project Structure

The repository is organized as follows:

```
RNNs-and-LSTMs-for-Text-Generation/
├── main.ipynb  # Jupyter Notebook containing the full tutorial and code
├── LICENSE                             # MIT License file
├── README.md                           # This README file with all steps included
└── requirements.txt                    # Required packages
```

## Detailed Tutorial Steps

### Introduction and Background

- Learn about sequence models and why RNNs are ideal for text generation.
- Understand the differences between RNNs, LSTMs, and GRUs.

### Dataset Preparation

- Use a unique dataset (*Ancient Myths: A Collection of Global Legends*) to train the model.
- Preprocess the text by converting to lowercase, creating character-to-index mappings, and generating sequences.

### Model Building

- Define a function to build an LSTM model in TensorFlow/Keras.
- Customize the architecture by adjusting the number of LSTM layers and units.
- Understand the significance of `return_sequences` in stacking LSTM layers.

### Training and Evaluation

- Train the model with a specified number of epochs.
- Generate text by sampling predictions with a temperature parameter.
- Evaluate the model's output and observe the effect of different settings.

### Experimenting with Model Depth

- Compare a baseline model (1 LSTM layer) with a deeper model (3 LSTM layers).
- Visualize training loss curves to understand the training dynamics.
- Compare the coherence of generated text between different architectures.

### Conclusion and Further Work

- Summarize the learning outcomes and how the model can be further improved.
- Discuss potential enhancements such as increased training, hyperparameter tuning, or alternative architectures.

## References

- Goodfellow, I., Bengio, Y., & Courville, A. (2016). *Deep Learning*. MIT Press.
- Olah, C. (2015). Understanding LSTM Networks. [Online Resource].
- Chollet, F. (2018). *Deep Learning with Python*. Manning Publications.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.