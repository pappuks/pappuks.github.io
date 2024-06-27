# Topics
- Medical Images
    - Types / Modalities
    -  Greyscale
        - 8 bit
        - 12 bit
        - 16 bit
    - Color
        - 8 bit per channel
    - Why lossless compression?
        - Reduce Liability
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

# Medical Images: A Comprehensive Overview
Medical imaging is a cornerstone of modern healthcare, providing critical insights into the human body that aid in diagnosis, treatment planning, and monitoring. This article delves into the various types and modalities of medical images, the importance of greyscale and color representations, and the necessity of lossless compression to maintain data integrity and reduce liability.
## Types / Modalities of Medical Images
Medical imaging encompasses a variety of modalities, each suited for different diagnostic purposes:
1. **X-ray**: Utilizes ionizing radiation to capture images of bones and certain tissues.
2. **Computed Tomography (CT)**: Combines multiple X-ray images to create cross-sectional views of the body.
3. **Magnetic Resonance Imaging (MRI)**: Uses magnetic fields and radio waves to produce detailed images of soft tissues.
4. **Ultrasound**: Employs high-frequency sound waves to visualize internal organs and structures.
5. **Positron Emission Tomography (PET)**: Detects metabolic activity and is often used in oncology.
6. **Mammography**: Specialized X-ray for breast tissue examination.
## Greyscale Imaging
Greyscale images are fundamental in medical imaging, representing different intensities of light in shades of grey. The bit depth of a greyscale image determines the number of possible shades:
### 8-bit Greyscale
- **8-bit**: Offers 256 shades of grey (2^8), sufficient for many types of medical images but may lack detail in subtle variations.
### 12-bit Greyscale
- **12-bit**: Provides 4,096 shades of grey (2^12), offering greater detail and depth, crucial for more nuanced imaging like CT scans.
### 16-bit Greyscale
- **16-bit**: Delivers 65,536 shades of grey (2^16), capturing the most detail and is often used in high-resolution imaging modalities like MRI.
## Color Imaging
Color images in medical imaging are less common but are used in specific applications like Doppler ultrasound and certain types of endoscopy. These images typically use 8 bits per channel (red, green, and blue), resulting in 24-bit color depth, which can represent over 16 million colors.
### 8-bit per Channel
- **8-bit per channel**: Each color channel (red, green, blue) has 256 possible values, allowing for detailed and nuanced color representation.
## Why Lossless Compression?
### Reduce Liability
Lossless compression is crucial in medical imaging to ensure that no data is lost during the compression process. This is vital for maintaining the integrity of medical images, as even minor alterations can lead to misdiagnosis or incorrect treatment plans. Lossless compression reduces storage requirements while preserving the original image quality, thereby reducing liability and ensuring compliance with medical standards and regulations.
## Data Compression Techniques
Several data compression techniques are employed to achieve lossless compression:
### LZ77
- **LZ77**: A dictionary-based algorithm that replaces repeated occurrences of data with references to a single copy in a sliding window.
### RLE
- **Run-Length Encoding (RLE)**: Simplifies data by replacing sequences of the same value with a single value and a count, effective for images with large uniform areas.
### Huffman Coding
- **Huffman Coding**: Uses variable-length codes for different symbols based on their frequencies, optimizing the overall data size.
### Arithmetic Coding
- **Arithmetic Coding**: Encodes entire messages into a single number, achieving higher compression rates by considering the probability of sequences.
### FSE
- **Finite State Entropy (FSE)**: A modern, efficient entropy coding technique that balances speed and compression ratio.
## Image Compression
While lossy compression methods are not suitable for medical images due to potential data loss, lossless compression techniques are essential.
### Lossless Compression Techniques
#### Optimize for Image Characteristics
Effective lossless compression techniques often optimize for the specific characteristics of medical images:
##### DPCM
- **Differential Pulse Code Modulation (DPCM)**: Encodes the difference between successive pixel values, reducing redundancy and improving compression efficiency.
##### Wavelet Transform
- **Wavelet Transform**: Decomposes images into different frequency components, allowing for efficient compression by focusing on significant features.
##### High Pass / Low Pass Filtering
- **High Pass / Low Pass Filtering**: Separates high-frequency details from low-frequency background, enabling more effective compression by targeting the most critical information.

In conclusion, the field of medical imaging relies heavily on advanced techniques for capturing, processing, and compressing images. By understanding the various modalities, the importance of greyscale and color representations, and the necessity of lossless compression, healthcare professionals can ensure the highest standards of diagnostic accuracy and patient care.
    

