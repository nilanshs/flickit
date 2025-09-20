# ⚽ My Computer Vision Assignment

This is my assignment for analyzing a soccer training video.  
The video is from YouTube: https://www.youtube.com/watch?v=k9gRgg_tW24  

The goal was to detect when the player touches the ball with the left or right leg, try to guess ball rotation, and calculate the player's velocity at each touch.  
I also created an annotated video with overlays and a CSV file with results.

---

## What I Did
1. Downloaded the video.
2. Used **MediaPipe** to detect body keypoints (ankles).
3. Used **OpenCV** to find the ball (HoughCircles).
4. Checked distance between ball and ankles → decided Left or Right touch.
5. Counted total touches and saved them.
6. Used optical flow (OpenCV) to estimate ball rotation direction.
7. Calculated player velocity from hip movement (in pixels/sec).
8. Saved results into a CSV file and drew overlays on the video.

---

## Tools I Used
- Python 3
- OpenCV
- MediaPipe
- Pandas
- tqdm (for progress bar)

---

## How to Run
1. Install requirements:
   ```bash
   pip install opencv-python mediapipe pandas tqdm
