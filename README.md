# pdfMergerAndPicToPdfAndMerge.ipynb

# 📄 PDF and Image Merger Tool

![Python](https://img.shields.io/badge/Language-Python-blue) ![Jupyter Notebook](https://img.shields.io/badge/Platform-Jupyter%20Notebook-orange) ![PyPDF2](https://img.shields.io/badge/Library-PyPDF2-orange) ![FPDF](https://img.shields.io/badge/Library-FPDF-green) ![PIL](https://img.shields.io/badge/Library-PIL-red)

---

## 🚀 Project Overview

This project features a robust and user-friendly tool for merging multiple files into a single PDF document. Built in **Jupyter Notebook (.ipynb)**, it allows users to merge **PDFs and images** while maintaining proper formatting. It uses **PyPDF2** for merging and **FPDF & PIL** for image conversion.

🔹 **Multi-format Compatibility:** Supports merging of PDF files and various image formats (e.g., PNG, JPEG).  
🔹 **Customizable Output:** Allows users to arrange the order of files before merging for a tailored final document.  
🔹 **Easy to Use:** Intuitive interface designed for both beginners and advanced users.  
🔹 **Use Cases:** Ideal for combining scanned documents, organizing project reports, or creating photo albums in PDF format.  
🔹 **Automatic Cleanup:** Removes temporary image-based PDFs after merging.  

---

## 📂 Project Structure

```
📁 project_directory/
 ├── pdf_merger.ipynb  # Jupyter Notebook
 ├── sample_pdfs/      # Folder containing input PDFs
 ├── sample_images/    # Folder containing input images
 ├── output/           # Folder for merged PDF
```

---

## 🛠️ Installation & Setup

### 1️⃣ Install Dependencies
Ensure you have Python installed, then install the required libraries:
```sh
pip install PyPDF2 pillow fpdf notebook
```

### 2️⃣ Open Jupyter Notebook
Run the following command to launch Jupyter Notebook:
```sh
jupyter notebook
```
Then open `pdf_merger.ipynb` and run all cells.

### 3️⃣ Change Directory in Jupyter Notebook
If you need to change the working directory in Jupyter, follow these steps:

#### 📁 Navigate Through File Explorer
When opening Jupyter Notebook, browse to your desired directory using the file browser interface.

Alternatively, open Jupyter directly in the desired directory using:
```sh
jupyter notebook
```
This will launch Jupyter in the directory where you executed the command.

#### 🖥️ Change Directory Dynamically in the Notebook
If you've already opened a notebook and want to switch directories, use this:
```python
import os
os.chdir('path/to/your/directory')  # Replace with the full path
print("Current Working Directory:", os.getcwd())
```

#### ⚡ Use the `%cd` Magic Command
Another quick way to switch directories within a notebook:
```python
%cd path/to/your/directory
```

---

### 4️⃣ Usage Instructions
Modify the script to specify your own input files:
```python
pdf_files = ["Doc.pdf", "news.pdf"]
image_files = ["pic.jpg"]
output_directory = "./output"
output_merged_pdf = "Merged_Result.pdf"
merge_pdfs_and_images(pdf_files, image_files, output_directory, output_merged_pdf)
```

---

## 🏗️ Functionality

### 📄 Merging PDFs
Uses `PyPDF2.PdfMerger()` to combine multiple PDF files while preserving their format.

### 🖼️ Image to PDF Conversion
- Converts images (JPEG, PNG) to A4-sized PDFs using **FPDF** and **PIL**.
- Maintains the aspect ratio to prevent distortion.
- Resizes images based on A4 dimensions (~210x297 mm).

### 🗑️ Cleanup
- Removes temporary image-based PDFs after merging.

---

## 📌 Example Output
After execution, the merged PDF is saved as:
```
output/Merged_Result.pdf
```

---

## 🤝 Contributing
💡 Feel free to fork, improve, and contribute to this project!  
📬 Contact: udvipmaurya@gmail.com

---

## 📜 License
📝 UDVIP License - Free to use and modify.

---

🌟 **If you find this project useful, please star ⭐ the repository!**

