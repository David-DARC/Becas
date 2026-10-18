# Becas
cd frontend
mkdir -p lib modelos

# Descargar la librería (solo el .min.js que es el que se usa)
wget https://cdn.jsdelivr.net/npm/face-api.js@0.22.2/dist/face-api.min.js -O lib/face-api.min.js

Descargar los modelos de IA
cd frontend/modelos

# TinyFaceDetector (detección rápida)
wget https://cdn.jsdelivr.net/gh/justadudewhohacks/face-api.js@master/weights/tiny_face_detector_model-weights_manifest.json
wget https://cdn.jsdelivr.net/gh/justadudewhohacks/face-api.js@master/weights/tiny_face_detector_model-shard1

# FaceLandmark68 (68 puntos del rostro)
wget https://cdn.jsdelivr.net/gh/justadudewhohacks/face-api.js@master/weights/face_landmark_68_model-weights_manifest.json
wget https://cdn.jsdelivr.net/gh/justadudewhohacks/face-api.js@master/weights/face_landmark_68_model-shard1

# FaceRecognition (vector de 128 números)
wget https://cdn.jsdelivr.net/gh/justadudewhohacks/face-api.js@master/weights/face_recognition_model-weights_manifest.json
wget https://cdn.jsdelivr.net/gh/justadudewhohacks/face-api.js@master/weights/face_recognition_model-shard1

cd backend
npm install //esto es para el sevidor node

permisos
chmod +x start.sh

correrlo en terminal
./start.sh

