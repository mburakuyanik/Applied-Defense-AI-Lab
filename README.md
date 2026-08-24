```markdown
# Applied Defense AI Lab

Hands-on implementations, models, and pipelines built for defense-oriented AI workloads—focusing on Computer Vision, RAG architectures, and Sensor Fusion.

---

##  Overview

This repository contains reproducible Jupyter notebooks and standalone scripts covering tactical AI use cases:

* **Perception & Tracking:** Object detection and multi-target tracking under real-time constraints.
* **LLM & Knowledge Retrieval:** Deterministic RAG pipelines and function calling for mission documentation.
* **Sensor Fusion:** Filtering and state estimation across noisy sensor telemetry.

---

##  Repository Structure

```
├── LLM-RAG/
│   ├── 01_rag_chunking_embeddings.ipynb      # Recursive splitting & context overlap
│   ├── 02_vectordb_chroma_cosine.ipynb        # Vector search with ChromaDB & metric evaluations
│   ├── 03_prompt_hallucination_prevention.ipynb # Strict grounding & zero-temp configurations
│   └── 04_agentic_tool_calling.ipynb          # Tool calling & ReAct decision loop
│
├── ComputerVision-ObjectDetection-YOLO/
│   ├── 01_iou_metric_calculation.ipynb        # Custom IoU, Precision, Recall & mAP calculations
│   ├── 02_yolo_inference_nms.ipynb            # YOLOv8 inference pipeline & NMS thresholding
│   └── 03_object_tracking_bytetrack.ipynb     # ByteTrack / DeepSORT tracking & ID management
│
└── Sensor-Fusion/ (In Progress)
    ├── 01_kalman_filter_sensor_fusion.ipynb   # 1D/2D Kalman Filter state estimation
    └── 02_imu_gps_fusion.ipynb                # IMU + GPS telemetry fusion

```

---

##  Core Focus Areas

### 1. Computer Vision & Target Tracking

* **Detection:** YOLOv8 integration for aerial/ground asset identification with optimized inference parameters.
* **Metrics:** Custom IoU implementation, confusion matrix metrics, and mAP evaluation curves.
* **Tracking:** Multi-Object Tracking (MOT) leveraging ByteTrack and DeepSORT logic to prevent ID switches during occlusions.

### 2. LLMs, RAG & Agents

* **Chunking Strategies:** Semantic-preserving text splitting with overlap tuning to prevent information loss.
* **Embeddings & Search:** Vector indexing with ChromaDB using cosine similarity.
* **Reliability:** System-level prompt constraints to eliminate hallucinations in technical query answering.
* **Tool Calling:** Interfacing LLM outputs directly with Python functions for deterministic mathematical execution.

### 3. Sensor Fusion & Navigation

* **State Estimation:** Discrete Kalman Filter implementation for position/velocity tracking.
* **Multi-Modal Data:** Combining low-rate GPS telemetry with high-rate IMU acceleration data.

---

##  Quick Run

All notebooks are self-contained and run directly in Google Colab (GPU recommended for YOLO workflows).

To run locally:

```bash
git clone [https://github.com/mburakuyanik/Applied-Defense-AI-Lab.git](https://github.com/mburakuyanik/Applied-Defense-AI-Lab.git)
cd Applied-Defense-AI-Lab

pip install torch torchvision ultralytics chromadb langchain-text-splitters opencv-python filterpy

```

---

##  Stack

* **Language:** Python 3.10+
* **Frameworks:** PyTorch, Ultralytics (YOLO), LangChain
* **Databases & Tools:** ChromaDB, OpenCV, NumPy, SciPy, FilterPy

```

```
