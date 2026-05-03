# OpenCV Face AR Filter 

A real-time augmented reality face filter built with OpenCV that detects faces and overlays custom images (like eyes and nose) on top of them.

---

##  Features
- Real-time face detection using Haar Cascade
- Custom image overlays (eyes + nose)
- Transparent PNG support (alpha blending)
- Dynamic resizing based on face size
- Webcam-based live processing

---

##  How It Works

This project detects faces in a live webcam feed and places custom images on specific facial regions.

Workflow:
1. Capture webcam frame
2. Detect face using Haar Cascade
3. Calculate approximate positions for:
   - Eyes
   - Nose
4. Resize overlay images based on face size
5. Blend PNG overlays with transparency
6. Render final augmented frame

---

## Required Files

Make sure you have these files in your project directory:

haarcascade_frontalface_default.xml

ball.png

nose.png

### Important:

PNG images must include transparency (alpha channel)

---

##  Controls

Press ESC to exit

---

## Output

Blue rectangles show detected face area

Ball images are placed over eyes 

Nose image is placed over nose area 

Everything scales dynamically with face size

---

## Key Concepts Used

Face detection (Haar Cascade)

Image resizing based on geometry

Alpha blending (transparent PNG overlay)

Coordinate mapping on face regions

 ---
 
## Technical Notes

Eye positions are approximated using fixed ratios of face width/height

Overlay function respects image boundaries

Alpha channel is used to handle transparency correctly

Face size determines scaling of all overlays
