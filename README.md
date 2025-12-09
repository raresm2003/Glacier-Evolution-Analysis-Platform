# 🌍 Automatic Glacier Evolution Analysis  
### Satellite Imagery Processing + Residual U-Net Deep Learning

This project implements my bachelor thesis, presenting a full system for **automatic glacier detection and long-term evolution analysis** using satellite imagery and convolutional neural networks.

## 🚀 Overview
- Residual U-Net deep learning model (TensorFlow → ONNX)
- Node.js backend for satellite image retrieval, inference, and data processing
- React + Next.js frontend for visualization and geospatial analysis

## 🧠 Deep Learning Model
- Architecture: Residual U-Net  
- Dataset: HKH Glacier Mapping Dataset  
- Loss: Dice Loss  
- Export: ONNX  
- Performance: ~87% accuracy, Dice ≈ 0.65

## 🛰 Satellite Image Workflow
1. Retrieve yearly Sentinel Hub images  
2. Filter by cloud coverage and season  
3. Select best RGB image  
4. Run ONNX inference  
5. Compute glacier area (km²)  
6. Save images, masks, overlays, metadata

## 🏗 Architecture
### Backend
- Node.js + Express  
- Python ONNX inference  
- Deterministic processing pipeline  

### Frontend
- React + Next.js  
- Leaflet map  
- Recharts graphs  
- Year slider visualization  

## 🛠 Installation

### Backend
cd glacier-backend  
npm install  

### Python
cd ml  
python3 -m venv venv  
source venv/bin/activate  
pip install -r requirements.txt  

Create `.env` with Sentinel credentials.

Start backend:
node index.js

### Frontend
cd glacier-evolution-app  
npm install  
npm run dev  

## 📈 Outputs
- Satellite RGB  
- Segmentation mask  
- Overlay  
- Glacier area graph  
- Metadata JSON  

## 👤 Author
Rareș Miclea  
Bachelor Thesis — 2025
