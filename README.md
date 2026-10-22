# ✈️ AeroScan AI: Automated Aircraft Structural Damage Classification & Captioning Suite

Welcome to the Aircraft Damage Inspection Project! This project utilizes Computer Vision and Vision-Language models to classify, caption, and summarize aircraft surface damage (Crack and Dent).

📌 Project Overview
This project is designed to make aircraft safety inspection fast and automated:

CNN Damage Classification: Uses a deep learning model to check images and identify whether the defect is a Crack or a Dent.

BLIP Text Generation: Leverages a pretrained BLIP model to generate automated captions and structural summary reports.

Visual Damage Overlay: Draws a bounding box overlay on the image to highlight high-risk damaged regions.

JSON Audit Report: Live exports inspection results in a formatted JSON structure.

🚀 Key Features
Dual AI Inference: A seamless combination of TensorFlow (CNN Classification) and PyTorch Transformers (BLIP Captioning).

Gradio Dashboard UI: A dark-themed web interface where you can upload images directly to run live inspections.

Automated Summary Logs: Provides detailed confidence scores, primary defect classification, and maintenance recommendations.

🛠️ How to Run on Google Colab
Install Dependencies:pip install gradio tensorflow torch transformers pillow numpy

Run the Notebook:
Execute all Colab Notebook cells sequentially so that both the CNN and BLIP models are loaded into memory.

Launch Gradio:
Execute the Gradio code cell and click on the generated public link to access your dashboard!

📋 Sample Output Structure
JSON
{
    "Inspection_ID": "AERO-1710000000",
    "Primary_Defect": "Crack",
    "Confidence_Score": "94.20%",
    "Caption": "A close up photo of a visible crack along the metallic panel of an aircraft fuselage.",
    "Summary": "Structural fracture detected requiring non-destructive testing (NDT) and immediate patch repair."
}
📜 License
MIT License - Available for open-source and educational use.



                           
