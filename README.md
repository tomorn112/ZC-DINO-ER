## 🥚 ZC-DINO-ER
This repository contains the supplementary code for the journal submitted to **IEEE Access (2025)** titled:  
**"Zero-Shot Eggshell Crack Detection Using Grounding DINO and FFT-Based Outer-to-Inner Ring Energy Ratio"**

---

## 📂 Dataset Structure

- `dataset1_images/hen/`  
  Contains **50 hen egg trays** captured from various angles. This is the **primary dataset** used for crack vs. intact classification and model training.

- `dataset2_videos/`  
  Contains **real-world video footage** used for evaluating the robustness of the detection pipeline in dynamic, practical scenarios.

- `duck_egg_dataset/`  
  Additional dataset contributed by Bhavya Botta and Ashis Kumar Datta for real-time crack detection on duck eggs.  
  📎 [View on Figshare](https://figshare.com/articles/dataset/Dataset_for_real-time_crack_detection_on_chicken_eggs/21568425)

---

## 📘 Code Structure (organized by GitHub branches)

The code is divided into **4 branches**, each representing a phase of the detection pipeline:

| Branch   | Description |
|----------|-------------|
| `part1`  | 🧼 **Crop and remove background** from egg tray images using segmentation techniques |
| `part2`  | 🧠 Use **Grounding DINO with fine-grained prompts** and **Ring Outer/Inner Energy Ratio** to differentiate between cracked and intact eggs |
| `part3`  | 📊 **Compare** performance with traditional **supervised learning models** (e.g., CNN, SVM) and **segmentation models** |
| `part4`  | 🎥 Perform **real-world video testing** using `dataset2_videos` to evaluate generalizability and inference speed |

---

## 🔧 Requirements & Dependencies

Each branch includes its own notebook and environment, but the general requirements include:

- Python 3.8+
- PyTorch
- torchvision
- Grounding DINO
- OpenCV
- scikit-learn

---

## 📬 Contact

For questions, collaboration, or discussion, feel free to open an issue or contact the maintainer.

---
