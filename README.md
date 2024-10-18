# Topic Modeling with LDA

This project implements a topic modeling algorithm using Latent Dirichlet Allocation (LDA) on a collection of text reviews. The code processes text data, tokenizes words, removes noise and stop words, and visualizes the frequency distribution of tokens.

## Dependencies

- `nltk`
- `sklearn`
- `numpy`

## Functions

### `list_of_tokens(reviews)`
- **Description**: Processes a list of reviews by removing noise, tokenizing words, and removing stop words.
- **Input**: `reviews` - A list of text reviews.
- **Output**: A list of cleaned and tokenized words.

### LDA Model
- The code uses the `LatentDirichletAllocation` from `sklearn` to fit the model on the processed text data.
- **Parameters**:
  - `n_components`: Number of topics to extract (set to 8).
  - `learning_method`: Method for updating the model (set to "online").
  - `max_iter`: Maximum number of iterations (set to 30).
  - `random_state`: Seed for random number generation (set to 2022).

## Usage

1. Prepare your text reviews in a list format.
2. Call `list_of_tokens(reviews)` to process the reviews.
3. Fit the LDA model to your transformed text data.
4. The output will display the frequency distribution of tokens and the topics identified by the LDA model.


