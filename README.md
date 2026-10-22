# ✈️ AeroScan AI: Automated Aircraft Structural Damage Classification & Captioning Suite

> **An advanced multimodal AI dashboard combining Deep Convolutional Neural Networks (CNN) and Vision-Language Models (BLIP) for automated aircraft structural integrity inspection.**

---

## 📌 Project Overview

Manual structural inspection of commercial aircraft fuselages is time-consuming and subject to human fatigue. **AeroScan AI** provides an automated visual inspection and diagnostic framework:

1. **Defect Classification:** Classifies structural panel defects into high-risk categories (`Crack` vs `Dent`) using a deep CNN backbone.
2. **Multimodal Captioning & Summarization:** Leverages the **BLIP (Bootstrapping Language-Image Pre-training)** vision-language model to generate human-readable diagnostic descriptions and maintenance summaries.
3. **Visual Bounding Overlays:** Draws dynamic highlight bounding regions around identified defects.
4. **Automated Inspection Reporting:** Generates audit-ready JSON inspection logs with severity levels and confidence scores.

---

## 🚀 Key Features

* **Dual AI Inference Pipeline:** Combines TensorFlow/Keras vision models with PyTorch Transformers.
* **Interactive Gradio Dashboard:** Dark-themed UI for instant upload and URL analysis.
* **Bounding Overlay Highlights:** Visual indicator highlighting damaged zones (`Crack` in Red, `Dent` in Orange).
* **Automated JSON Audit Logs:** Generates real-time structured logs containing Inspection ID, confidence scores, and recommended actions.
* **Google Colab Ready:** Easily deployable in cloud GPU environments.

---

## 🏗️ System Architecture

┌───────────────────────────────┐
                           │     Input Aircraft Photo      │
                           └───────────────┬───────────────┘
                                           │
                           ┌───────────────┴───────────────┐
                           │                               │
                           ▼                               ▼
          ┌─────────────────────────────────┐   ┌─────────────────────────────────┐
          │     Deep CNN Classifier         │   │   BLIP Multimodal Transformer   │
          │   (Classify: Dent vs Crack)     │   │  (Captioning & Summarization)   │
          └────────────────┬────────────────┘   └────────────────┬────────────────┘
                           │                                     │
                           └───────────────┬─────────────────────┘
                                           │
                                           ▼
                           ┌───────────────────────────────┐
                           │   Interactive Gradio Suite    │
                           │   - Visual Bounding Overlay   │
                           │   - Probability Distribution  │
                           │   - JSON Log Report           │
                           └───────────────────────────────┘
## 🛠️ Installation & Setup

### Prerequisites
- Python 3.10 or higher
- GPU support recommended (CUDA/Google Colab T4)

## Sample Output

{
    "Inspection_ID": "AERO-1710000000",
    "Primary_Defect": "Crack",
    "Confidence_Score": "94.20%",
    "AI_Generated_Caption": "A close up photo of a visible crack along the metallic panel of an aircraft fuselage.",
    "AI_Structural_Summary": "Structural fracture detected requiring non-destructive testing (NDT) and immediate patch repair.",
    "Recommended_Action": "Immediate NDT Testing & Repair Patch"
}



                           
