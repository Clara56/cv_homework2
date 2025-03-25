# cv_homework2
image processing : cartoon rendering project using OpenCV

# 🎨 Cartoonization and Pencil Sketch Effect  

This project applies **cartoonization** and **pencil sketch effects** to images and videos using **OpenCV**. It enhances images by preserving edges while smoothing colors, creating a cartoon-like appearance.  

## 📌 Features  
✅ Convert images to cartoon-style drawings  
✅ Generate realistic pencil sketches from images  
✅ Live webcam cartoonization  
✅ Adjustable parameters for customization  

---

## 📥 Installation  
### **1️⃣ Install Dependencies**  
Make sure you have Python installed, then install the required libraries:  
```bash
pip install opencv-python numpy
```
  
### **2️⃣ Run the Cartoonization**  
```bash
python main.py
```
- Replace `"image.jpg"` with your own image file.  
- Uncomment `cartoonize_video()` to apply the effect to a **live webcam feed**.  

---

## 📸 Demo  

### ✅ **Images that Work Well**  
Our algorithm performs best on images with:  
- **Strong edges** (e.g., portraits, well-defined objects).  
- **Vibrant colors** that allow for good contrast.  
- **Good lighting** (sharp details).  

---

### ❌ **Images that Do Not Work Well**  
The algorithm struggles with images that have:  
- **Low contrast or poor lighting** → weak edge detection.  
- **Blurry or noisy images** → edges become unclear.  
- **Overly complex textures** (e.g., forests, detailed patterns).  

---
## some output
![pencil_sketch](https://github.com/user-attachments/assets/90334a36-dfb1-48cd-97f9-8a378fd49d8d)

![cartoonized_image](https://github.com/user-attachments/assets/0a9aa4dc-c8f4-4ad1-92e4-332d788f6a36)

---

## 🔍 Limitations  

### ⚠ 1. Loss of Fine Details  
- Small details (like facial expressions) may be lost due to edge simplification.  

### ⚠ 2. Over-Smoothing  
- The **bilateral filter** reduces noise but sometimes **blurs important details**.  

### ⚠ 3. Sensitivity to Lighting & Contrast  
- **Dark images** result in **weak edge detection**, making the cartoon effect less clear.  

### ⚠ 4. Real-Time Performance Issues  
- The **bilateral filter is computationally expensive**, making live webcam processing slow on low-end devices.  

---

## 📚 Future Improvements  
🔹 **Use Deep Learning** for better edge detection.  
🔹 **Improve Real-Time Performance** by optimizing filters.  
🔹 **Enhance Parameter Adjustability** for user control.  

---

## ✨ Credits  
Developed using **OpenCV** and **NumPy**.  

🚀 *Enjoy cartoonizing your images and videos!* 🚀  
