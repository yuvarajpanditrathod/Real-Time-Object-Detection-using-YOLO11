# 🖼️🎯 Real-Time Object Detection System using YOLO11  

![Python](https://img.shields.io/badge/Python-3.8%2B-green?logo=python&logoColor=white) ![YOLO](https://img.shields.io/badge/YOLO-v11-red?logo=github&logoColor=white)  ![OpenCV(https://img.shields.io/badge/OpenCV-Enabled-blue?logo=opencv&logoColor=white) ![Status](https://img.shields.io/badge/Status-Active-success)  



A modern, professional web application for real-time object detection using YOLO11 models built with **Flask** backend and **Bootstrap** frontend. This system provides live webcam detection, image analysis, and video processing capabilities with a sleek, responsive web interface.

## Technology Stack

- **Backend**: Flask (Python web framework)
- **Frontend**: HTML5 + Bootstrap 5 for responsive design
- **AI/ML**: YOLO11 (Ultralytics) for object detection
- **Computer Vision**: OpenCV for image/video processing
- **Deep Learning**: PyTorch backend

## Features

### 🎥 Live Webcam Detection
- Real-time object detection using your camera
- Optimized for performance with YOLOv11m model
- Live FPS counter and statistics
- Start/stop controls

### 📸 Image Detection
- Upload and analyze static images
- High-accuracy detection with YOLOv11x model
- Drag & drop file upload
- Results display with bounding boxes
- Detection count statistics

### 🎬 Video Processing
- Upload and process video files
- Frame-by-frame object detection
- Progress tracking
- Support for multiple video formats

### 🎨 Professional Interface
- Modern, responsive web design with Bootstrap 5
- Clean and intuitive user interface
- Real-time status indicators
- Progress tracking and statistics
- Error handling and user feedback
- Mobile-friendly responsive design
- Cross-browser compatibility

## Installation

### Prerequisites
- Python 3.10 or higher
- Webcam (for live detection)
- At least 4GB RAM recommended

### Quick Start
1. Clone or download this repository
2. Follow the manual installation steps below
3. Open your browser to `http://localhost:5000`

### Manual Installation
1. Clone Repository:
   ```bash
   git clone https://github.com/yuvarajpanditrathod/Real-Time-Object-Detection-using-YOLO11.git
   cd Real-Time-Object-Detection-using-YOLO11
   ```
3. Create a virtual environment:
   ```bash
   python -m venv .venv
   ```

2. Activate the virtual environment:
   ```bash
   # Windows
   .venv\Scripts\activate
   
   # Linux/Mac
   source .venv/bin/activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the application:
   ```bash
   python Yolo11-Object-Detection.py
   ```

## Configuration

The application uses configuration settings directly in the main Python file. You can modify settings such as:

- Model paths (currently uses yolo11x.pt and yolo11m.pt)
- Confidence thresholds for detection
- Upload and result folder paths
- Camera settings

## Models

The application uses two YOLO11 models:
- **yolo11x.pt**: High-accuracy model for image/video processing
- **yolo11m.pt**: Medium model optimized for real-time webcam detection

Models are automatically downloaded on first run.

## API Endpoints

- `GET /` - Main application interface
- `GET /video_feed` - Live webcam stream for real-time detection
- `POST /detect_image` - Image detection endpoint
- `POST /detect_video` - Video detection endpoint with streaming results

## Supported Formats

### Images
- JPG, JPEG, PNG, BMP
- Drag & drop upload support
- Base64 encoded results display

### Videos
- MP4, AVI (common video formats)
- Real-time frame processing
- Streaming detection results

## Features in Detail

### Object Detection
- Support for 80+ COCO dataset classes including:
  - Vehicles: car, bicycle, motorcycle, airplane, bus, train, truck, boat
  - People and animals: person, bird, cat, dog, horse, sheep, cow, elephant
  - Objects: bottle, cup, laptop, cell phone, book, chair, TV, etc.
- Real-time confidence scoring
- Bounding box visualization with class labels

### Performance Optimizations
- Dual model system: yolo11x.pt for accuracy, yolo11m.pt for speed
- Optimized camera capture settings
- JPEG compression for video streaming
- Efficient frame processing
- Memory management for large files

### File Management
- Automatic directory creation (uploads/, results/)
- Temporary file storage system
- Base64 image encoding for web display
- Safe file handling and cleanup
- Flask-based file upload handling

### Web Interface
- Bootstrap 5 responsive design
- Interactive file upload with drag & drop
- Real-time video streaming
- Dynamic result display
- Mobile-optimized layout
- Professional styling and animations

### Testing
- Automated system testing with Selenium
- Web interface testing capabilities
- Error handling validation

## Troubleshooting

### Common Issues

1. **Camera not working**
   - Check camera permissions in your browser
   - Ensure no other application is using the camera
   - Try restarting the application
   - Verify camera index (default is 0)

2. **Models not loading**
   - Check internet connection (models download automatically on first run)
   - Ensure sufficient disk space (models are ~100MB total)
   - Verify model files exist in project directory

3. **Performance issues**
   - Close other GPU/CPU intensive applications
   - Lower confidence threshold in the code
   - Use yolo11m.pt model for faster processing

4. **File upload errors**
   - Verify file format is supported (JPG, PNG, MP4, AVI)
   - Check file permissions
   - Ensure sufficient disk space

5. **Port already in use**
   - Change port in `app.run()` to a different port
   - Kill existing Flask processes

### Testing the Application
- Use the provided test images and videos in the `uploads/` folder
- Run `Testing/System-Testing.py` for automated testing
- Check `results/` folder for detection outputs

### Getting Help
- Enable Flask debug mode by setting `debug=True`
- Check browser console for JavaScript errors
- Verify all dependencies are installed: `pip list`

## Sample Files

The project includes sample test files in the `uploads/` directory:
- **Images**: cars.jpg, cat.jpg, plants.jpg, vegitables.jpg, etc.
- **Videos**: demo.mp4, test_video.mp4, car.mp4, etc.

These files can be used to test the detection functionality without uploading your own content.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## Acknowledgments

- Ultralytics for the YOLO11 models
- Flask framework for web development
- Bootstrap 5 for responsive UI design
- OpenCV for computer vision operations
- PyTorch for deep learning backend
- COCO dataset for object classes

---

## 👨‍💻 Developer

**Made with ❤️ by [Yuvaraj](mailto:yuvarajpanditrathod@gmail.com)**


*This project was developed as a demonstration of modern web technologies combined with cutting-edge AI for object detection. Feel free to contribute and make it even better!*
*"Building the future, one line of code at a time!"* - Yuvaraj
#






