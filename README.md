![WhatsApp Image 2025-10-18 at 15 02 01_24f640e5](https://github.com/user-attachments/assets/425a5459-d377-4d70-805d-38cf93b85a87)<p align="center">
 <img width="538" height="318" alt="image" src="https://github.com/user-attachments/assets/9cf87f49-59e0-4f05-af9b-ca51970b8ca3" />
</p>

<h1 align="center">Density-Based-Traffic-Optimization</h1>

<div align ="center">

[![Python version](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)

<h4>This research project presents an AI-based adaptive traffic signal control system using YOLOv5 and OpenCV for real-time vehicle density estimation and emergency vehicle prioritization. The system dynamically adjusts signal timing based on traffic conditions, reducing congestion and improving emergency response time.</h4>

</div>

### 🌍 Inspiration

* With rapid urbanization and the rise in private vehicles, **traffic congestion** has become a severe issue in metropolitan cities. It leads to increased **travel time**, **fuel consumption**, and **air pollution**.

* According to the [TomTom Traffic Index](https://www.tomtom.com/en_gb/traffic-index/ranking/), cities like **Mumbai** and **Bengaluru** rank among the most congested in the world, where traffic jams can reach over **70% congestion** during peak hours.

* Traditional traffic control systems rely on fixed timers that do not adapt to real-time traffic conditions. This results in inefficient flow and long waiting times at intersections.

* To overcome these limitations, our proposed **Density-Based Traffic Optimization System** uses **YOLOv5** and **computer vision** to detect real-time vehicle density, allocate dynamic green times, and prioritize emergency vehicles such as ambulances.

------------------------------------------

### ⚙️ Implementation Details

This project can be divided into **four major modules**:

1. **Vehicle Detection Module**  
   Detects and classifies vehicles (cars, bikes, buses, trucks, rickshaws) from live camera feeds using a fine-tuned YOLOv5 model.

2. **Density Calculation & Adaptive Control**  
   Calculates lane-wise vehicle density and dynamically adjusts the green signal time using the formula:  

   \[
   GST = \frac{\sum (NoOfVehicles_{class} \times AvgTime_{class})}{(NoOfLanes + 1)}
   \]

3. **Emergency Vehicle Priority Module**  
   Detects ambulances in real-time and immediately provides a **green corridor**, halting other lanes to ensure smooth emergency clearance.

4. **Simulation Module**  
   Developed using the [Pygame](https://www.pygame.org/) library to visualize adaptive signal control, vehicle flow, and ambulance prioritization in real-time.

📘 *Read more about our implementation and methodology in the paper accepted at CIACON 2025. View the Paper [here](https://ieeexplore.ieee.org/document/11189675).*

------------------------------------------
### 🧠 Results & Highlights

| Metric | Static System | Proposed System |
|--------|----------------|----------------|
| Detection Accuracy | 80% | **94.7%** |
| Vehicle Throughput | Baseline | **+36%** |
| Emergency Clearance Time | Standard | **37% Faster** |
| Delay Reduction | None | **23% Lower Idle Time** |

✅ The proposed model effectively improves traffic flow and ensures quicker emergency responses, making it a scalable and cost-efficient solution for smart cities.

------------------------------------------
### 🧩 System Workflow

<p align="center">
 <img height=300px src="./assets/workflow-diagram.png" alt="System Workflow">
</p>

**Step 1:** Live traffic feed captured from CCTV cameras.  
**Step 2:** YOLOv5 model detects and classifies vehicles.  
**Step 3:** Density data is processed to determine optimal signal durations.  
**Step 4:** In case of ambulance detection, system activates priority clearance.  
**Step 5:** Real-time updates displayed through simulation.

------------------------------------------
### 🧰 Tech Stack

| Component | Technology |
|------------|-------------|
| Programming Language | Python 3.8+ |
| Object Detection | YOLOv5 (PyTorch) |
| Image Processing | OpenCV |
| Simulation | Pygame |
| Data Handling | NumPy, Pandas |

------------------------------------------
### 💻 Demo

*Vehicle Detection*

<p align="center">
 <img height=400px src="./assets/vehicle-detection.png" alt="Vehicle Detection">
</p>

<br>

*Adaptive Signal Simulation*

<p align="center">
 <img src="./assets/demo.gif" alt="Traffic Simulation">
</p>

------------------------------------------

### 🧾 Publication & Recognition

1) **Interraction With Government Authority :**  
We visited **local government authorities** to present our project and demonstrate **how the density-based traffic optimization system works using YOLO**. This discussion focused on **potential real-world deployment and traffic management integration**.

<p align="center">
  <img src="![WhatsApp Image 2025-10-18 at 15 02 01_24f640e5](https://github.com/user-attachments/assets/67878be7-0909-4404-a262-49ec71f55260)
" alt="Government Interaction" width="600"/>
</p>

2) **Research Paper Publication:**  
Our paper based on this project, **"Density-Based Traffic Optimization Using YOLO"**, was presented at **CIACON 2025** and published in **IEEE Xplore**. The paper details our methodology, experiments, and results for adaptive traffic signal optimization.
📄 View the Paper [here](https://ieeexplore.ieee.org/document/11189675).

------------------------------------------

 👥 Contributors

| Name               | Role                           |
|-------------------|--------------------------------|
| Sankalp Tirpude    | Lead Developer & Researcher    |
| Samiksha Dhawale   | Co-Researcher                  |
| Purva Rathi        | Simulation & Analysis          |
| Priyanshu Rodge    | Implementation & Testing       |
| Dr. Vibha Bora     | Project Guide & Supervisor     |

###  Acknowledgement
We sincerely thank **Dr. Vibha Bora**, our project guide, for her continuous guidance, valuable insights, and encouragement throughout this research.  
Special thanks to the **Department of Electronics Engineering, G.H. Raisoni College of Engineering, Nagpur** for providing resources and support.

### 🪪 License
This project is licensed under the **MIT License** – see the [LICENSE](./LICENSE) file for details.

### 📬 Contact
**Email:** sankalptirpude2003@gmail.com  
**LinkedIn:** [Sankalp-Tirpude](https://www.linkedin.com/in/sankalp-tirpude-1b015a247/).

---

<h4 align="center">⭐ If you found this project helpful, consider starring the repository and sharing it!</h4>
