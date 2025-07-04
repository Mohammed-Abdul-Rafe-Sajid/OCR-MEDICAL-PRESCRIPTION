
# 📝 Handwritten Medical Prescription OCR System

This project is part of my AI/ML research internship capstone, aiming to develop an intelligent system that reads and extracts meaningful data from handwritten medical prescriptions using OCR and basic machine learning techniques.

## 📌 Project Objective

To build a system that can:
- Read handwritten medical prescriptions using OCR.
- Extract structured information such as:
  - Medicine names
  - Dosage (e.g., 500mg)
  - Frequency (e.g., twice a day)

---

## 🧠 Technologies & Tools Used

- **Language:** Python
- **Libraries/Frameworks:**
  - OpenCV (Image Preprocessing)
  - Tesseract OCR (Text Recognition)
  - NumPy, Pandas (Data Handling)
  - Regex / NLP (Text Parsing)
  - (Optional) TensorFlow or PyTorch (Deep Learning Enhancement)
- **Platform:** Google Colab / Jupyter Notebook

---

## 📂 Project Structure
├── data/
│ ├── raw/ # Raw prescription images
│ └── processed/ # Preprocessed (cleaned) images
├── notebooks/
│ └── main_pipeline.ipynb # Core project steps
├── outputs/
│ └── extracted_text.csv # OCR + structured results
├── README.md
└── requirements.txt


---

## 🔄 Workflow

1. **Data Collection:** Use of real or synthetic handwritten prescription images.
2. **Image Preprocessing:** Resize, grayscale, denoise, and threshold images for better OCR.
3. **Text Recognition:** Apply Tesseract OCR to extract raw text from images.
4. **Text Parsing:** Clean and structure the OCR output using string processing and regex.
5. **(Optional)** Deep Learning Enhancement using CNNs to detect specific fields (medicine name, dosage).

---

## ✅ Sample Output

**Input Image:**

*insert image here*

**Extracted Output:**
```json
{
  "Medicine": "Paracetamol",
  "Dosage": "500mg",
  "Frequency": "Twice a day"
}

📈 Future Improvements
Use deep learning to improve accuracy on poor handwriting.

Build a web app using Streamlit for user interaction.

Integrate with a drug database for verification.

📚 References
Tesseract OCR Documentation

OpenCV Tutorials

Kaggle Medical OCR Datasets

🙋‍♂️ Author
Mohammed Abdul Rafe Sajid
AI/ML Research Intern
Chaitanya Bharathi Institute of Technology

