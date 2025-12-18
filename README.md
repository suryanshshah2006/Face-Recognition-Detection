# Face-Recognition-Detection
Real-Time Face Recognition & Detection System

A high-performance face recognition system that combines multiple state-of-the-art Deep Learning architectures to detect and identify faces in live video streams or static images.

🧠 Architecture & Methodology

Detection: Utilized MTCNN (Multi-task Cascaded Convolutional Networks) for robust face detection even in varying orientations.

Embeddings: Used InceptionResnetV1 (pretrained on VGGFace2) to generate 128-dimensional facial embeddings.

Recognition: Implemented Euclidean distance-based classification to match live embeddings against a known database.

Preprocessing: Integrated OpenCV for grayscale conversion, image resizing, and bounding box visualization.

🛠️ Tech Stack

Frameworks: PyTorch, Facenet-PyTorch.

Computer Vision: OpenCV.

Support: Numpy, Pillow (PIL), Matplotlib.

🚀 How it Works

Detect faces using MTCNN.

Generate facial embeddings for each detected face.

Compare embeddings with the "known" face database.

If distance < threshold, label the face; otherwise, mark as "Unknown."
