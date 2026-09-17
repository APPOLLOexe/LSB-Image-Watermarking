# LSB-Image-Watermarking
Web-based image watermarking application using Flask, OpenCV, and LSB steganography for embedding and extracting digital watermarks.
Original Image
      │
      ├───────────────┐
      │               │
      ▼               ▼
Cover Image       Watermark
      │               │
      │          Resize + Grayscale
      │               │
      │          Convert to 3-bit
      │               │
      └───────┬───────┘
              ▼
      LSB Embedding
              │
              ▼
    Blue Channel Modified
              │
              ▼
       Watermarked Image
              │
              ▼
       LSB Extraction
              │
              ▼
      Reconstructed Watermark
