# HTTP Code Retrieval Library

Contains the 13 non-empty code cells from the supplied Colab notebook, each saved as an individual `.py` file. Each source file was verified against its original code cell character-for-character.

## One-time hosting setup
1. Create a **public** GitHub repository.
2. Upload the 13 `.py` files from this folder to the repository root. (You do not need to upload the notebook or README.)
3. The raw URL base follows this format: `https://raw.githubusercontent.com/USERNAME/REPOSITORY/main/`
4. Open `HTTP_Code_Retrieval.ipynb` and replace `USERNAME/REPOSITORY` in `BASE_URL`. Keep the trailing slash.
5. Run the setup cell.

## Retrieve source code
```python
list_codes()
get_code(1)
get_code('4.1')
get_code(5)
get_code('cnn_l1')
```

The code is fetched over HTTPS from GitHub and displayed; it is not executed. Copy it into a separate cell to run. `urllib` is part of Python's standard library; no pip installation is needed.

## Constraints
- Internet access is required at retrieval time. The Jupyter kernel makes an HTTPS request; no browser tab is opened.
- The repository must be public for this no-authentication setup.
- If the college network blocks `raw.githubusercontent.com`, this method will fail; test before the exam.
- Running the retrieved programs may need their original ML libraries and datasets. Retrieval itself does not.

## Original program mapping
- Program 1: Deep Forward ANN (`deep_forward_ann.py`)
- Program 2: MNIST Deep Feedforward (`mnist_deep_feedforward.py`)
- Program 3: Fashion MNIST CNN (`fashion_mnist_cnn.py`)
- Program 4.1: Basic CNN (`basic_cnn.py`)
- Program 4.2: CNN with L1 (`cnn_l1.py`)
- Program 4.3: CNN with L2 (`cnn_l2.py`)
- Program 4.4: CNN with Dropout (`cnn_dropout.py`)
- Program 4.5: CNN with L2 + Dropout (`cnn_l2_dropout.py`)
- Program 5: BLIP Image Captioning (`blip_image_captioning.py`)
- Program 6: Bidirectional LSTM (`bidirectional_lstm.py`)
- Program 7: MNIST Autoencoder (`mnist_autoencoder.py`)
- Program 8: MNIST GAN (`mnist_gan.py`)
- Program 10: Simple RNN (`simple_rnn.py`)
