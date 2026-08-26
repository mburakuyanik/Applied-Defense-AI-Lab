Markdown
# Applied Defense AI Lab

Hands-on implementations, models, and pipelines built for defense-oriented AI workloads—focusing on Computer Vision, RAG architectures, and Sensor Fusion.

---

## 🎯 Overview

This repository contains reproducible Jupyter notebooks covering core defense and security AI concepts:

* **Perception & Tracking:** Real-time object detection (YOLOv8) and multi-target tracking (ByteTrack) under occlusion scenarios.
* **Generative AI & RAG:** Grounded document retrieval with ChromaDB, Cosine Similarity, strict hallucination prevention, and agentic tool calling.
* **Sensor Fusion & Edge AI:** Discrete/Extended Kalman Filtering (EKF), visual navigation principles, ONNX conversion, and time-series telemetry anomaly detection.

---

## 📂 Repository Structure

```text
├── ComputerVision-ObjectDetection-YOLO/
│   ├── iou_metric_calculation.ipynb        # Custom IoU, Precision, Recall & evaluation logic
│   ├── yolo_inference_nms.ipynb            # YOLOv8 inference pipeline & NMS thresholding
│   └── object_tracking_bytetrack.ipynb     # ByteTrack tracking & persistent ID association
│
├── LLM-RAG/
│   ├── rag_chunking_embeddings.ipynb       # Recursive text splitting & context overlap
│   ├── vectordb_chroma_cosine.ipynb        # ChromaDB vector indexing & cosine similarity search
│   ├── prompt_hallucination_prevention.ipynb # Strict grounding & zero-temperature constraints
│   └── agentic_tool_calling.ipynb          # Autonomous agent planning & Python tool calling
│
└── SensorFusion-AutonomousSystems/
    ├── kalman_filter_simulation.ipynb      # 1D Kalman Filter state estimation & noise filtering
    ├── multi_sensor_fusion_ekf.ipynb       # Multi-sensor fusion (IMU + Visual Odometry) via EKF
    └── edge_optimization_anomaly.ipynb     # ONNX model export & telemetry anomaly detection (Z-Score)
🚀 Key Modules & Technical Capabilities
1. Computer Vision & Target Tracking
Object Detection: YOLOv8 inference pipeline optimized for speed and recall.

Metrics: Ground-truth vs prediction IoU calculations, confidence filtering, and Non-Maximum Suppression (NMS).

Multi-Object Tracking (MOT): Temporal identity preservation and occlusion handling via ByteTrack.

2. LLMs, RAG & Agentic Systems
Chunking & Embeddings: Recursive text splitting with overlap tuning to prevent contextual degradation.

Semantic Search: Vector indexing with ChromaDB using cosine similarity metrics.

Hallucination Mitigation: System-prompt engineering and zero-temperature configurations for deterministic technical QA.

Agentic Workflows: Function calling mechanisms enabling LLMs to execute exact mathematical and sensor tools.

3. Sensor Fusion & Edge AI
State Estimation: Discrete Kalman Filter and Extended Kalman Filter (EKF) models for position and velocity estimation.

GNSS-Denied Navigation: Multi-modal sensor integration combining high-rate IMU data with visual odometry.

Edge Optimization: PyTorch model conversion to ONNX format for low-latency embedded inference.

Anomaly Detection: Statistical Z-Score modeling on real-time telemetry streams.

🛠️ Stack & Dependencies
Languages: Python 3.10+

Deep Learning & Vision: PyTorch, Ultralytics (YOLOv8), OpenCV

NLP & Vector DB: LangChain, ChromaDB, Sentence-Transformers

Math & Filtering: NumPy, Matplotlib, SciPy
