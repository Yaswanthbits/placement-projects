# SOP-3-1 Complete Project Structure

This document outlines the complete file structure of the SOP-3-1 Chess Board Recognition System project, available in the original repository at [mr-robot-2211/SOP-3-1](https://github.com/mr-robot-2211/SOP-3-1).

## Directory Structure

```
SOP-3-1/
├── dataset/
│   └── train/              # Training dataset directory
│                           # Contains chess piece images for training
│
├── outputs/                # Model output results (variant 1)
├── outputs2/               # Model output results (variant 2)
├── outputs3/               # Model output results (variant 3)
├── outputs4/               # Model output results (variant 4)
│
├── Core Training & Model Files:
├── train.py                # CNN model training script
├── CNN_model.py            # Convolutional Neural Network architecture
├── chess_piece_detector.h5 # Trained neural network model (H5 format)
│
├── Image Preprocessing Scripts:
├── part1.py                # Image preprocessing part 1
├── part1_2.py              # Image preprocessing part 2
├── piece_to_square.py      # Convert individual piece to square
├── 2_pieces_to_squares.py  # Convert 2-piece images to squares
├── 3_pieces_to_squares.py  # Convert 3-piece images to squares
├── 4_pieces_to_squares.py  # Convert 4-piece images to squares
├── 5_pieces_to_squares.py  # Convert 5-piece images to squares
├── 6_pieces_to_squares.py  # Convert 6-piece images to squares
│
├── Prediction & Detection Scripts:
├── predict.py              # Chess piece prediction (version 1)
├── predict2.py             # Chess piece prediction (version 2)
├── predict3.py             # Chess piece prediction (version 3)
│
├── Integration & Visualization:
├── combine_final.py        # Final pipeline integration script
├── final_blender_script.py # Blender 3D visualization integration
│
├── Configuration Files:
├── pieces.txt              # Chess piece class definitions
├── pieces2.txt             # Alternative piece definitions
│
├── Sample Output Files:
├── output2.jpg             # Sample prediction output
├── reconstructed_board.jpg # Example reconstructed chess board
│
├── Temporary/Debug:
├── tempCodeRunnerFile.py   # Temporary debug file
│
└── Documentation:
    ├── README.md           # Main project readme
    └── PROJECT_STRUCTURE.md # This file
```

## File Categories

### 1. Training & Model Development
- **train.py**: Main training script that trains the CNN on chess piece dataset
- **CNN_model.py**: Neural network architecture definition
- **chess_piece_detector.h5**: Saved trained model in Keras/TensorFlow format

### 2. Data Preprocessing
Scripts that convert raw chess images into standardized square format:
- **part1.py, part1_2.py**: Initial image preprocessing
- **piece_to_square.py**: Base conversion utility
- **N_pieces_to_squares.py**: Batch conversion scripts for varying piece counts

### 3. Prediction & Inference
Scripts that use the trained model to detect chess pieces:
- **predict.py, predict2.py, predict3.py**: Different prediction implementations

### 4. Pipeline Integration
- **combine_final.py**: Combines all preprocessing, prediction, and reconstruction steps
- **final_blender_script.py**: Exports to Blender for 3D visualization

### 5. Configuration
- **pieces.txt, pieces2.txt**: Defines chess piece classes and labels

### 6. Output Folders
- **outputs/** to **outputs4/**: Store results from different experimental runs

## Key Components Workflow

```
Raw Chess Image
       ↓
   part1.py (preprocessing)
       ↓
N_pieces_to_squares.py (standardization)
       ↓
predict.py (detection using CNN)
       ↓
combine_final.py (integration)
       ↓
final_blender_script.py (3D visualization)
       ↓
Reconstructed Chess Board
```

## Technologies Stack

- **Deep Learning**: TensorFlow/Keras
- **Computer Vision**: OpenCV (cv2)
- **Image Processing**: NumPy, PIL/Pillow
- **3D Rendering**: Blender (Python API)
- **Language**: Python 3.7+

## Data Format

- **Training Data**: Image files (JPG/PNG)
- **Model**: HDF5 format (.h5)
- **Configuration**: TXT text files
- **Output**: JPG images, potentially Blender files (.blend)

## How to Access Full Source

All files and complete source code available at:
**https://github.com/mr-robot-2211/SOP-3-1**

This placement-projects folder contains documentation and key structural information for portfolio verification.
