# PowerLine-MTYOLO

Hy, Peace be upon you,

This repository contains the code, dataset links, and demo video for the paper:
"PowerLine-MTYOLO: A Multitask YOLO Model for Simultaneous Cable Segmentation and Broken Strands Detection", currently under submission to MDPI Drones.

📜 Abstract
Power transmission infrastructure requires continuous inspection to prevent faults and ensure grid stability. UAV-based systems, enhanced with deep learning, have emerged as an efficient alternative to traditional, labor-intensive inspection methods. However, existing approaches typically rely on separate models for cable segmentation and anomaly detection, increasing computational overhead and reducing reliability in real-time applications.

To address these limitations, we propose PowerLine-MTYOLO, a lightweight, one-stage multitask model designed for simultaneous power cable segmentation and broken strand detection from UAV imagery. Built upon the A-YOLOM architecture and leveraging the YOLOv8 foundation, our model introduces four specialized modules—SDPM, HAD, EFR, and Shape-Aware WiseIoU loss—to improve geometric understanding, structural consistency, and bounding box precision.

We also release the Merged Public Power Cable Dataset (MPCD), a diverse open-source dataset tailored for multitask training and evaluation. Experimental results show that PowerLine-MTYOLO achieves up to +10.68% mAP50 and +1.7% IoU over A-YOLOM, while outperforming recent YOLO-based detectors in both accuracy and efficiency. These gains are achieved with a smaller model footprint and the same inference speed as A-YOLOM.

🎥 Video Demonstration
Watch a real-world test of PowerLine-MTYOLO in Morocco (Casablanca) on unseen UAV footage:

🧪 Google Colab - Reproduce Our Results
You can run the full inference or training pipeline via Google Colab :

📊 Dataset: Merged Public Power Cable Dataset (MPCD)
We aggregate and relabel 5 public Roboflow datasets for multitask training, resulting in:

1,871 images

2,501 cable segment masks

1,906 broken cable annotations



💻 Code Availability


📄 License
This project is licensed under the GNU Affero General Public License v3.0 (AGPL-3.0).

🙏 Acknowledgments
We thank the Ultralytics YOLO team for providing the foundation upon which PowerLine-MTYOLO is built.
We also acknowledge the Roboflow community for the datasets that helped us create MPCD.
And also A yolo M for ...

📌 Citation
Once published, please cite the paper using the following format (to be updated): 
