# Rail-Crossing Safety Project

This repository is the main entry point for the **Rail-Crossing Safety Project**, an AI-driven solution designed to improve safety at railway crossings using computer vision, edge computing, and real-time alerts. The project is split into two submodules for better modularity and scalability.

![Watch the video](assets/0114.gif)

## Repository Structure

### Submodules:

1. **[Railway Demo App](https://github.com/muntakim1/railway_demo_app):**

   - Handles real-time video processing and object detection at railway crossings.
   - Integrates YOLOv8 for vehicle, pedestrian, and signal detection.
   - Provides visualization with bounding boxes and hazard alerts.

2. **[MT Edge](https://github.com/muntakim1/mt-edge):**
   - Optimized for edge devices like Jetson Nano.
   - Manages deployment and ensures low-latency real-time processing.
   - Includes edge-specific configurations and scripts.

## Key Features

- **Real-Time Detection:** Uses YOLOv8 to identify vehicles, pedestrians, and signals.
- **Proactive Alerts:** Automated detection of unsafe scenarios, triggering alerts for immediate response.
- **Edge Deployment:** Tested and deployed on Jetson Nano for efficient real-time processing.
- **Custom Dataset:** Trained on rail-crossing-specific data to enhance detection accuracy.

## Technology Stack

- **YOLOv8:** Object detection model for precision and speed.
- **Python & OpenCV:** For video processing, visualization, and integration.
- **Jetson Nano:** Edge device for deployment and real-time performance.
- **Docker:** Ensures smooth deployment across environments.

## Getting Started

### Prerequisites

- Python 3.8 or above
- NVIDIA Jetson Nano (for edge deployment)
- Docker (optional, for containerized setup)

### Setup Instructions

1. Clone this repository:

   ```bash
   git clone --recurse-submodules https://github.com/muntakim1/rail-crossing-safety.git
   ```

2. Navigate to the submodules and follow their respective setup guides:

   - [Railway Demo App Setup](https://github.com/muntakim1/railway_demo_app#readme)
   - [MT Edge Setup](https://github.com/muntakim1/mt-edge#readme)

3. Train or fine-tune the YOLOv8 model if needed using your custom dataset (optional).

4. Deploy the application on your target device:
   - For local testing: Run the Railway Demo App.
   - For edge deployment: Use the MT Edge module on Jetson Nano.

## Usage

- **Local Deployment:**
  ```bash
  python app.py
  ```
- **Edge Deployment:**
  Follow the instructions in the [MT Edge](https://github.com/muntakim1/mt-edge#readme) repository.

## Contributions

Contributions are welcome! If you would like to contribute to the project, please:

- Fork the repository.
- Make changes in a separate branch.
- Submit a pull request with detailed explanations of your changes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contact

For questions, suggestions, or feedback, please feel free to reach out or open an issue in this repository.
