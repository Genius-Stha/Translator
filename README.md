# SEQUENCE TO SEQUENCE
In this project i have applied encoder-decoder and Transformer architecture for english to spanish translation where the encoder and decoder block contains LSTM blocks for processing and Transformer block contains attention mechanism for sequence to sequence translation. The model is trained on a large dataset of English to Spanish sentences and then evaluated on a test set to measure its performance. The model is able to translate English sentences into Spanish with high accuracy and fluency. The model is also able to handle out-of-vocabulary words by using a pre-trained word embedding.
## ENCODER DECODER
The encoder-decoder architecture is a common approach for sequence to sequence translation. In this architecture, the encoder takes the input sequence and produces a context vector, which is then passed to the decoder. The decoder takes the context vector and the input sequence, and generates the output sequence. The encoder-decoder architecture is simple and easy to implement, but it can be slow for long sequences.

Here i have coded entire encoder and decoder block without using any library. The code is written in python and uses LSTM blocks for processing and Transformer block contains attention mechanism for sequence to sequence translation. The model is trained on a large dataset of English to Spanish sentences and then evaluated on a test set to measure its performance. The model is able to translate English sentences into Spanish with okey translation because i have only trained it for 10 epochs.

**Encoder**

![encoder](/img/encoder.png)

**Decoder**

![decoder](/img/decoder.png)

**seq2seq model**

![seq2seq](/img/enc-dec-model.png)


## Transformer
The transformer architecture is a more advanced approach for sequence to sequence translation. This was first introduced in the paper "Attention is All You Need" by Vaswani et al. in 2017. The transformer architecture is based on the idea of self-attention, which allows the model to focus on different parts of the input sequence at the same time. The transformer architecture is much more powerful than the encoder-decoder architecture, but it is also more complex to implement.

I have implemented exact replica of the transformer model from the paper "Attention is All You Need" by Vaswani et al. in 2017.

This model was also trained for 10 epoch and got much better translation accuracy than the encoder-decoder model.

The model contains different class of
- scaled_dot_product_attention
- FeedForward
- EncoderLayer
- DecoderLayer
- TransformerEncoder
- TransformerDecoder
- Transformer
- TranslationDataset


**Parameters**

![transformer-parameters](/img/transformer_parameters.png)

