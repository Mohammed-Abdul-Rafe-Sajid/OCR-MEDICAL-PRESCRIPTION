# 📝 Handwritten Medical Prescription OCR System

This project was developed as part of my **AI/ML Research Internship Capstone** under the mentorship of **Mr. Rammakrishna Sir**.
The goal was to design an intelligent OCR-based system capable of reading and extracting structured data from **handwritten medical prescriptions**, an especially challenging domain in computer vision and natural language processing.

---

## 📌 Project Objective

To build a system that can:

* Recognize and extract text from handwritten medical prescriptions.
* Identify key structured entities such as:

  * **Medicine names**
  * **Dosage** (e.g., 500mg)
  * **Frequency** (e.g., twice a day)

---

## 🧠 Technologies & Tools Used

* **Language:** Python
* **Libraries & Frameworks:**

  * **OpenCV** – for image preprocessing (grayscale, denoising, thresholding)
  *  **Tesseract OCR** – for traditional optical character recognition
  *  **EasyOCR** – deep learning–based OCR for comparison
  *  **TRoCR (Transformer-based OCR)** – tested but did not yield strong results on limited handwritten data
  *  **NumPy**, **Pandas** – for data handling
  *  **Regex / NLP** – for post-processing and text structuring
* **Environment:** Google Colab

---

## 🔄 Workflow

1. **Data Collection**

   * 129 real-world handwritten medical prescription images (.jpg format).
   * Collected from local clinics and public medical note samples.

2. **Preprocessing (OpenCV)**

   * Resize → Grayscale → Gaussian Blur → Otsu’s Threshold
   * Improved readability for OCR models by enhancing text clarity.

3. **OCR Extraction**

   * **Tesseract OCR** used with `--oem 3` and `--psm 6` for block text mode.
   * **EasyOCR** tested for deep learning–based recognition.
   * **TRoCR (Microsoft Research)** tried but required more data and fine-tuning to perform effectively.

4. **Post-processing**

   * Regex and string parsing applied to clean text and identify medicine, dosage, and frequency patterns.
   * Extracted results stored in `.txt` format for each image.

---

## 📊 Key Observations & Learnings

* **OCR Accuracy** heavily depends on **image preprocessing** and **page segmentation modes**.
* **Handwritten prescriptions**, due to inconsistent handwriting and overlapping text, remain a major OCR challenge.
* **Tesseract** performed better for structured printed text, while **EasyOCR** handled cursive handwriting marginally better.
* **TRoCR**, though advanced, did not generalize well due to limited training data and high handwriting variability.
* Established a **baseline OCR pipeline** that can later be improved using CNN/RNN-based recognition and entity extraction models.

---

## 🚀 Future Work

* Fine-tune **EasyOCR** or **TRoCR** models on a **custom medical handwriting dataset**.
* Integrate **Named Entity Recognition (NER)** for structured extraction of medicine names and dosage patterns.
* Explore **Vision Transformers (ViT)** or **CNN-based encoders** for better handwritten text understanding.

---

## 🙋‍♂️ Author

**Mohammed Abdul Rafe Sajid**
- Research Intern
Chaitanya Bharathi Institute of Technology

