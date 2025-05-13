# NeuroDetect - Object Detection using YOLOv8 and Streamlit

A streamlined application for object detection and tracking using YOLOv8, integrated with an interactive dashboard powered by Streamlit. This project combines cutting-edge object detection algorithms with an intuitive interface to provide real-time analytics for images and videos.

---

## About the Project

### Problem Statement
Object detection and tracking are critical components in computer vision with applications ranging from surveillance systems to industrial automation. However, existing tools often lack user-friendly interfaces and require significant technical expertise to operate.

### How This Project Solves It
This project offers:
1. **Ease of Use**: A clean, intuitive dashboard for uploading videos or images, selecting object classes to detect, and visualizing results.
2. **Interactivity**: Provides options to download detection data for further analysis, making it ideal for users without extensive technical knowledge.

## How to Run the Project

### Prerequisites
Ensure the following are installed on your system:
- Python 3.8+
- Streamlit
- Plotly
- PIL
- OpenCV
- Ultralytics (YOLOv8)

### Steps to Run

1. Clone the repository:

```bash
git clone https://github.com/sagar1024/NeuroDetect-Object-Detection-using-Streamlit.git
cd NeuroDetect-Object-Detection-using-Streamlit
```

2. Launch the Streamlit app:

```bash
streamlit run app.py
```

3. Access the app in your browser at http://localhost:8501.

## How the Project Works

### Image Mode:

1. Upload an image file.

2. Perform object detection for selected classes.

3. Visualize results directly on the dashboard.

### Video Mode:

1. Upload a video file.

2. Select object classes and confidence threshold from the sidebar.

3. View detections in real-time, with bounding boxes drawn on detected objects.

## Dashboard Features:

Real-time visualizations of detected objects.

Interactive charts and download options for detection statistics.

## Challenges Faced and How We Overcame Them

1. Video Playback Issues:
Initially faced problems with autoplay functionality for embedded videos. Resolved by converting the demo video to a GIF and using st.image for seamless playback.

2. Handling Large Files:
Uploading large videos/images caused performance lags. Mitigated this by resizing input files dynamically using OpenCV.

3. Real-Time Detection Rendering:
Streamlit's default rendering posed challenges for displaying real-time detections. Solved this by leveraging Streamlit's st.image and efficiently updating frames.

## Future Enhancements

1. Add support for additional object detection models.

2. Enable real-time webcam feed for live detections.

3. Expand analytics capabilities with more advanced visualization tools.

