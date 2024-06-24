# Topics
- Medical Images
    - Types / Modalities
    -  Greyscale
        - 8 bit
        - 12 bit
        - 16 bit
    - Color
        - 8 bit per channel
- Data Compression
    - LZ77
    - RLE
    - Huffman
    - Arihmetic Coding
    - FSE
- Image Compression
    - Lossy (we are not going to talk about this)
    - Lossless (our focus is this)
    - Techniques
        - Optimize for image characteristics
            - DPCM
            - [Wavelet Transform](./lossless-wavelet-transform.md)
            - High Pass / Low Pass filtering 
- Medical Image Codec
    - Lossless, optimized for 16 bit images
    - Uses Optimized DPCM, Optimized RLE and FSE
    - All algorithms have been optimized for 16 bit data 
    

