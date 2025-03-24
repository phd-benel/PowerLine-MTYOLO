# PowerLine-MTYOLO

Hy, Peace be upon you,

This repository contains the code, dataset links, and demo video for the paper:
"PowerLine-MTYOLO: A Multitask YOLO Model for Simultaneous Cable Segmentation and Broken Strands Detection", currently under submission to MDPI Drones.

# 📜 Abstract

Power transmission infrastructure requires continuous inspection to prevent faults and ensure grid stability. UAV-based systems, enhanced with deep learning, have emerged as an efficient alternative to traditional, labor-intensive inspection methods. However, existing approaches typically rely on separate models for cable segmentation and anomaly detection, increasing computational overhead and reducing reliability in real-time applications.

To address these limitations, we propose PowerLine-MTYOLO, a lightweight, one-stage multitask model designed for simultaneous power cable segmentation and broken strand detection from UAV imagery. Built upon the A-YOLOM architecture and leveraging the YOLOv8 foundation, our model introduces four specialized modules—SDPM, HAD, EFR, and Shape-Aware WiseIoU loss—to improve geometric understanding, structural consistency, and bounding box precision.

We also release the Merged Public Power Cable Dataset (MPCD), a diverse open-source dataset tailored for multitask training and evaluation. Experimental results show that PowerLine-MTYOLO achieves up to +10.68% mAP50 and +1.7% IoU over A-YOLOM, while outperforming recent YOLO-based detectors in both accuracy and efficiency. These gains are achieved with a smaller model footprint and the same inference speed as A-YOLOM. By unifying detection and seg-25 mentation into a single framework, PowerLine-MTYOLO offers an interesting solution for 26 autonomous aerial inspection and provides a foundation for future advancements in fine-27 structure monitoring tasks.

 # 🎥 Video Demonstration

[![Watch the video](https://github.com/user-attachments/assets/edbccd9c-1082-46ca-bbdb-7344cebc93aa)](https://drive.google.com/file/d/1BAyHy7wOnVeD2ZADb3s6ebX8UoOnylSc/view?usp=sharing)


The UAV footage shown in the demo video was not included in the training dataset (MPCD). This "unseen data" was used exclusively for visual evaluation, demonstrating PowerLine-MTYOLO’s ability to generalize to new and diverse real-world inspection scenarios.


# 🧪 Google Colab - Reproduce Our Results

You can run the full inference (Here are the pretrained weights https://github.com/phd-benel/PowerLine-MTYOLO/blob/main/PowerLine-MTYOLO-NANO-150Epochs.pt) or training pipeline via Google Colab :

# 📊 Dataset: Merged Public Power Cable Dataset (MPCD)

We aggregate and relabel 5 public Roboflow datasets for multitask training, resulting in:

1,871 images

2,501 cable segment masks

1,906 broken cable annotations

https://drive.google.com/file/d/1KyciMmwL2_p_-mwckHFqG5fkBA1jzATv/view?usp=sharing

# 💻 Code Availability

https://drive.google.com/file/d/1FJP-EsAv12IhYyOiIy1K9Q-DL5mUpn-X/view?usp=drive_link

# 📄 License
This project is licensed under the GNU Affero General Public License v3.0 (AGPL-3.0).

# 🙏 Acknowledgments
We thank the Ultralytics YOLO team for providing the foundation upon which PowerLine-MTYOLO is built. We also acknowledge the Roboflow community for the open-source datasets that enabled the construction of the Merged Public Power Cable Dataset (MPCD). Additionally, we extend our appreciation to the authors of A-YOLOM [Wang et al., 2023, GitHub: https://github.com/JiayuanWang-JW/YOLOv8-multi-task] for their pioneering work in multitask learning, which served as the architectural basis and inspiration for our proposed framework.

# 📌 Citation
Once published, please cite the paper using the following format (to be updated): 
