# HR Vision

A real-time face recognition dashboard for HR purposes with WebRTC and Socket.IO streaming.

## Features

- Real-time face recognition using InsightFace and TensorFlow
- Multiple camera streaming options (WebRTC, Socket.IO)
- Mobile camera integration via QR code scanning
- Employee attendance tracking
- Dashboard with analytics
- PostgreSQL integration

## Technology Stack

- Backend: FastAPI, Python
- Real-time Communication: WebRTC (aiortc), Socket.IO
- Face Recognition: InsightFace, TensorFlow
- Database: PostgreSQL
- Frontend: HTML, CSS, JavaScript

## Setup Instructions

1. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Copy `env_template.txt` to `.env` and update with your database credentials

4. Run the application:
   ```bash
   uvicorn main:app --host 0.0.0.0 --port 8000 --reload
   ```

## Camera Integration

The system supports multiple camera types:

1. **WebRTC Camera**: Low-latency streaming with built-in statistics
2. **Mobile Camera**: Turn any mobile device into a camera using QR code scanning
3. **Local Webcam**: Use your computer's webcam

## Face Recognition System

To set up the face recognition system:

1. Create a directory for face images (e.g., `eagles/faces`)
2. Create subdirectories for each person (e.g., `eagles/faces/John`)
3. Add multiple face images (JPG, JPEG, or PNG) for each person
4. Run the face recognition script to generate embeddings

## License

MIT