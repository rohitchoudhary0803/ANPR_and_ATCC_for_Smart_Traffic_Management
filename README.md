# ANPR and ATCC for Smart Traffic Management

## Project Overview
This project is focused on developing an intelligent traffic management system using Automatic Number Plate Recognition (ANPR) and Automatic Traffic Classification and Control (ATCC). By utilizing Deep Learning and Object Detection techniques, the system automates traffic monitoring and control in smart city environments.
- ANPR is used to detect and recognize vehicle license plates.
- ATCC is used to classify different types of traffic.
The ultimate goal of this project is to improve traffic flow, reduce congestion, and enhance road safety in urban areas.

### Key Features
-  Automatic Number Plate Recognition (ANPR)
-  Automatic Traffic Classification and Control (ATCC)
-  Data interpolation for accurate tracking
-  Visualization capabilities

### Result
- Result videos : "[Click Here For Video 1](https://drive.google.com/file/d/1YHDEWEz84UbcPJToZjzTVGw28Wil6qK7/view?usp=drive_link)" and "[Click Here For Video 2](https://drive.google.com/file/d/1bvG9D3B7p4hQByGwAQDQEYI9nWeSlSY3/view?usp=drive_link)".

## Folder Structure
The following directory structure is used in this project:
```
├── CV_Basics/                  # Basic learning of Computer Vision and OCR
├── Data/                        # Input data or videos
├── Interpolated_results/        # Interpolated CSV files for visualization
├── number_plate_detection_model_training/   # Files related to model training
├── object_tracker/              # Main file for vehicle detection and tracking
├── output_videos/               # Output videos generated after visualization
├── results/                     # CSV files for interpolation
├── testing/                     # Testing files for various project modules
├── .env                         # Contains secret keys
├── .gitignore                   # Git ignored files and folders
├── add_missing_data.py          # Interpolation of data for accurate detection and visualization
├── main.py                      # Main script to run the system
├── requirements.txt             # Project dependencies
└── visualize.py                 # Visualize the output video using interpolated data
```

## Workflow
1. Execute `main.py` to perform initial vehicle detection and generate CSV file in `results/` directory
2. Run `add_missing_data.py` to perform data interpolation and generate enhanced CSV file in `Interpolated_results/` directory
3. Run `visualize.py` to create visualization video using interpolated data, saved in `output_videos/` directory

## Installation
1. Clone the repository:
```bash
git clone https://github.com/rohitchoudhary0803/Smart-Traffic-Management
cd Smart-Traffic-Management
```

2. Create and activate virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Configure environment variables:
- Create a copy of `.env.example` (if provided) and rename it to `.env`
- Update the necessary secret keys and configurations

## How to Run this project


1. Replace the path to your input video and your desired output directory.

2. Run the main detection:
```bash
python main.py
```

3. Perform data interpolation:
```bash
python add_missing_data.py
```

4. Generate visualization:
```bash
python visualize.py
```

## License
ANPR and ATCC for Smart Traffic Management is released under the [MIT License](LICENSE), allowing you to freely use, modify, and distribute the project.
