#lowlevel 

#### **[[Encoder]] Layer Components**
1. **Multi-Head Self-Attention Mechanism:** This component allows the encoder to focus on different parts of the input sequence by computing multiple attention scores in parallel (multiple heads). Each head captures different aspects of the relationships between words.

2. **Feed-Forward Network (FFN):** After the multi-head attention mechanism, each position in the sequence is passed through a fully connected feed-forward network. The FFN is applied identically to each position and consists of two linear transformations with a ReLU activation in between.

3. **Layer Normalization and Residual Connections:** Each sub-layer (i.e., the multi-head attention and FFN) in the encoder is followed by layer normalization and a residual connection. The residual connection helps in preventing vanishing gradients and allows the model to learn identity functions more easily.

#### **[[Decoder]] Layer Components**
1. **Masked Multi-Head Self-Attention Mechanism:** Similar to the encoder, but with a crucial difference: the attention is masked to prevent the decoder from attending to future positions in the sequence. This is necessary for autoregressive tasks like language generation, ensuring that each position only attends to earlier positions.

2. **Encoder-Decoder Attention:** This layer allows the decoder to focus on relevant parts of the input sequence by attending to the encoder's output representations. It acts as a bridge between the encoder and decoder, providing context from the input sequence to the decoder's generation process.

3. **Feed-Forward Network (FFN):** Similar to the encoder, each position is processed through an FFN.

4. **Layer Normalization and Residual Connections:** As with the encoder, each sub-layer in the decoder is followed by layer normalization and a residual connection.