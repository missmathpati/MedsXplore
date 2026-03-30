# MedsXplore – Unlock Medicinal Insights

> ⚖️ **Officially copyrighted by the Government of India (Feb 2024)**

> Converts raw medicine images into structured, multilingual medical insights using an OCR + NLP pipeline.

---

## **Overview**

MedsXplore is an end-to-end OCR + NLP system designed to extract and structure medicine information from unstructured inputs such as images of pills, strips, and packaging.

---

## **System Overview**

The pipeline processes raw image inputs and converts them into structured, user-consumable medical insights:

### **1. OCR Extraction**
- Utilizes Microsoft Azure Computer Vision API for text extraction  
- Applies image preprocessing (contrast adjustment, noise reduction) to improve OCR quality  

### **2. Entity Resolution & Matching**
- Matches extracted text against a curated dataset of ~11,000 medicines  
- Implements:
  - Exact string matching  
  - Partial matching (first 6-character heuristic) to handle OCR noise  
- Improves robustness for incomplete or noisy text  

### **3. Information Retrieval**
- Retrieves structured attributes:
  - Composition  
  - Usage  
  - Side effects  
  - Manufacturer details  
  - User reviews  

### **4. Post-processing & Normalization**
- Standardizes outputs across heterogeneous formats  
- Cleans OCR artifacts and resolves inconsistencies  

### **5. Multilingual & Accessibility Layer**
- Machine translation for multi-language support  
- Text-to-speech (TTS) for audio-based interaction  

---

## **Architecture Design**

OCR Extraction → Entity Matching → Data Retrieval → Transformation → Output Delivery  

This modular design enables:
- Independent optimization of each stage  
- Improved scalability and maintainability  
- Seamless integration with downstream applications  

---

## **Performance & Impact**

- Built on a dataset of ~11,000 medicines for broad coverage  
- Handles noisy OCR outputs through heuristic-based matching  
- Reduces user effort from manual search to single image-based query  
- Supports multilingual access and audio narration for accessibility  

---

## **Tech Stack**

- **Backend:** Python, Flask  
- **OCR:** Microsoft Azure Computer Vision API  
- **Frontend:** HTML, CSS, JavaScript  
- **Processing:** NLP + rule-based matching and normalization  

---

## **Key Features**

- Image-based medicine identification  
- Structured medical insights extraction  
- Multilingual support  
- Audio narration (TTS)  
- Direct redirection for medicine purchase  

---
