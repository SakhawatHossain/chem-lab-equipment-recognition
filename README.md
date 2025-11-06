# Chemistry Lab Image Dataset Covering 25 Apparatus Categories

This dataset contains 4,599 high-quality, annotated images of 25 commonly used chemistry lab apparatuses. The images, each containing structures in real-world settings, have been captured from different angles, backgrounds, and distances, while also undergoing variations in lighting to aid in the robustness of object detection models. Every image has been labeled using bounding box annotation in TXT (YOLO) format, alongside the class IDs and normalized bounding box coordinates making object detection more precise. The annotations and bounding boxes have been built using the Roboflow platform.

To achieve a better learning procedure, the dataset has been split into three sub-datasets: training, validation, and testing. The training dataset constitutes 70% of the entire dataset, with validation and testing at 20% and 10% respectively. In addition, all images undergo scaling to a standard of 640x640 pixels while being auto-oriented to rectify rotation discrepancies brought about by the EXIF metadata. The dataset is structured in three main folders - train, valid, and test, and each contains images/ and labels/ subfolders. Every image contains a label file containing class and bounding box data corresponding to each detected object.

The whole dataset features 6,960 labeled instances per 25 apparatus categories including beakers, conical flasks, measuring cylinders, test tubes, among others. The dataset can be utilized for the development of automation systems, real-time monitoring and tracking systems, tools for safety monitoring, alongside AI educational tools.

## 🧠 Model Training and Evaluation

All models were trained and evaluated using **open-source frameworks**:

- **YOLOv5–YOLOv12** (via [Ultralytics](https://github.com/ultralytics/ultralytics))  
- **RF-DETR (Roboflow DETR)** ([GitHub repo](https://github.com/roboflow/rf-detr.git))

**Results summary (mAP@50 > 0.90):**

| Model | Precision | Recall | mAP@50 |
|:------|:----------:|:-------:|:-------:|
| RF-DETR | 99.1% | 79.9% | **0.992** |
| YOLOv11 | 96.7% | 97.7% | **0.987** |
| YOLOv9 | 96.4% | 97.3% | 0.986 |
| YOLOv8 | 96.2% | 97.0% | 0.983 |
| YOLOv5 | 96.0% | 96.9% | 0.985 |

Hyperparameters and training configurations are detailed in the publication (Tables 8–9).

## 🔽 Download

📁 **Dataset Page**  
[Chemistry Lab Image Dataset on Figshare](https://figshare.com/articles/dataset/_b_Chemistry_Lab_Image_Dataset_Covering_25_Apparatus_Categories_b_/29110433)

📦 **Direct Download (280.44 MB)**  
[Download Dataset ZIP](https://figshare.com/ndownloader/files/44682395)

📄 **Dataset DOI**  
[https://doi.org/10.6084/m9.figshare.29110433.v3](https://doi.org/10.6084/m9.figshare.29110433.v3)

📄 **Paper DOI**  
[https://doi.org/10.1038/s41597-025-05952-3](https://doi.org/10.1038/s41597-025-05952-3)


## 📑 Citation

If you use this dataset or accompanying code, please cite the publication:

```bibtex
@article{hossain2025realworld,
  title        = {Real-world chemistry lab image dataset for equipment recognition across 25 apparatus categories},
  author       = {Hossain, Md. Sakhawat and Haque, Md. Sadman and Rahman, Md. Mostafizur and Mousum, Md. Mosaddik Mashrafi and Razzaque, Zobaer Ibn and Robin, Robiul Awoul and Rahman, Raiyan and Noor, Jannatun},
  journal      = {Scientific Data},
  volume       = {12},
  pages        = {1747},
  year         = {2025},
  publisher    = {Nature Portfolio},
  doi          = {10.1038/s41597-025-05952-3}
}
