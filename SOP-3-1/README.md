# SOP-3-1: Chess Board Recognition System

## Group Project

### Overview

This is a machine learning and computer vision project focused on recognizing chess pieces and board squares using Convolutional Neural Networks (CNN). The system combines deep learning with image processing to detect and reconstruct chess boards from images.

### Original Repository

- **Repository**: [mr-robot-2211/SOP-3-1](https://github.com/mr-robot-2211/SOP-3-1)
- **Original Author**: [mr-robot-2211](https://github.com/mr-robot-2211)
- **Collaborator**: Yaswanthbits (Group Member)

### Contributors

- **mr-robot-2211** (Project Creator)
- **Yaswanthbits** (Group Collaborator)

### Project Components

#### Core Scripts
- `train.py` - Model training script for CNN
- `CNN_model.py` - Convolutional Neural Network architecture
- `part1.py`, `part1_2.py` - Image preprocessing and preparation
- `predict.py`, `predict2.py`, `predict3.py` - Chess piece prediction modules
- `combine_final.py` - Final integration and output generation
- `final_blender_script.py` - Blender rendering integration

#### Data Processing
- `2_pieces_to_squares.py` - Convert 2-piece images to chess squares
- `3_pieces_to_squares.py` - Convert 3-piece images to chess squares
- `4_pieces_to_squares.py` - Convert 4-piece images to chess squares
- `5_pieces_to_squares.py` - Convert 5-piece images to chess squares
- `6_pieces_to_squares.py` - Convert 6-piece images to chess squares
- `piece_to_square.py` - Individual piece to square conversion

#### Data & Models
- `dataset/train/` - Training dataset directory
- `chess_piece_detector.h5` - Trained neural network model
- `pieces.txt`, `pieces2.txt` - Chess piece configuration files
- `output2.jpg`, `reconstructed_board.jpg` - Sample outputs

#### Output Directories
- `outputs/`, `outputs2/`, `outputs3/`, `outputs4/` - Model output results

### Technologies Used

- **Python** - 100%
- **Deep Learning**: TensorFlow/Keras
- **Computer Vision**: OpenCV
- **Image Processing**: NumPy, PIL
- **3D Rendering**: Blender (optional)

### Key Features

✓ Chess piece detection using CNN  
✓ Board square recognition and mapping  
✓ Image-to-square conversion pipeline  
✓ Model training and prediction  
✓ 3D board reconstruction capability  
✓ Blender integration for visualization  

### Attribution

This project is included in the placement-projects portfolio for placement verification purposes. The work demonstrates collaborative machine learning and computer vision skills. Both mr-robot-2211 and Yaswanthbits contributed to this project's development.

### How to Use

1. **Training**: Run `train.py` with your chess piece dataset
2. **Preprocessing**: Use piece-to-square scripts to prepare data
3. **Prediction**: Use `predict.py` variants to detect pieces
4. **Integration**: Run `combine_final.py` for complete pipeline
5. **Visualization**: Optionally use `final_blender_script.py` for 3D rendering

### Requirements

- Python 3.7+
- TensorFlow/Keras
- OpenCV (cv2)
- NumPy
- PIL/Pillow
- Blender (optional, for rendering)

### Complete Source Code

All source code and data files are available in the original repository:
[https://github.com/mr-robot-2211/SOP-3-1](https://github.com/mr-robot-2211/SOP-3-1)

This folder in placement-projects contains the key components and documentation for portfolio verification.
