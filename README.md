<p align="center">
  <img width="800" src="./figures/conecta_logo.png" />
</p> 

# An TinyML Incremental Learning Approach for Outlier Detection and Correction


### ✍🏾Authors:  [Pedro Andrade](https://github.com/pedrohmeiraa), [Morsinaldo Medeiros](https://github.com/Morsinaldo), [Ivanovitch Silva](https://github.com/ivanovitchm), [Marianne Diniz](https://github.com/MarianneDiniz), and [Daniel G. Costa](https://github.com/daniel-gcosta).


# 1. Abstract/Overview
The Internet of Things (IoT) is a paradigm where computing and networking capabilities are integrated into objects, connecting them to the Internet. It is recognized as an important and emerging technology field with vast potential for improving lives, enhancing industrial processes, and enabling real-time decision-making. As the number of connected objects increases, the infrastructure for processing and handling the large volume of data generated also grows. In response, Edge Computing has emerged as a concept where data processing occurs closer to the data source, alleviating the burden on central servers. This article explores the integration of Tiny Machine Learning (TinyML) algorithms into resource-constrained devices, such as microcontrollers, enabling efficient data processing and inference directly on low-power devices. By leveraging lightweight algorithms and model optimization techniques, TinyML offers benefits such as reduced latency, enhanced privacy, improved energy efficiency, and increased autonomy for devices operating in remote or disconnected environments. This article presents an outlier detection and correction algorithm based on TinyML for deployment on resource-constrained computing devices. The algorithm was implemented in an OBD-II scanner as a proof of concept, where a microcontroller acquires real-time vehicle data, identifies outliers, and performs necessary corrections.
  
For a better didactic exposition, the results will be presented in 3 notebooks:

 1. :notebook: Explaining the TEDA Algorithm: Outlier Detection
 2. :orange_book: Explaining the TEDA RLS Algorithm
 3. :green_book: Comparing Freematics, Arduino, C++ e Python

# 2. Environment Setup
First, start by cloning the repository:
```bash
git clone https://github.com/conect2ai/IEEE-SENSORS-2024-TEDARLS.git
```

We also have cloned the `Padasip` repository:
```bash
git clone https://github.com/matousc89/padasip
```
It is possible to install using `pip`:
```bash
!pip3 install padasip
```
- The **Padasip** (*Python Adaptive Signal Processing*) is a library designed to simplify adaptive signal processing tasks within Python (filtering, prediction, reconstruction, classification). More information [here](https://matousc89.github.io/padasip/).  :twisted_rightwards_arrows:

Now, we are going to install the  `WandB`: 💻

```bash
!pip3 install wandb -qU
```
 - If you want to know more about software package **WandB**, click [here](https://wandb.ai/site).  :bar_chart:
 
## 2.1 How to run on Freematics One+

1. Install [Visual Studio Code](https://code.visualstudio.com/)
2. Install [PlatformIO](https://platformio.org/) (VSCode Extension)
3. Clone this repository:

```bash
git clone https://github.com/conect2ai/IEEE-SENSORS-2024-TEDARLS.git
```

4. Open the project folder `./Freematics/firmware_v5/telelogger` on PlatformIO, as illustrated in the figure below.

<p align="center">
  <img width="800" src="./figures/platformio.png" />
</p> 

5. Connect the Freematics One+ to your computer and turn it on using the Freematics Emulator or in the vehicle.

6. Compile, upload and monitor the serial (steps 1, 2 and 3, respectively in the figure below).

<p align="center">
  <img width="800" src="./figures/upload.png" />
</p> 


# 3. References

 [[1]](https://www.mdpi.com/1424-8220/22/10/3838) :books: **Andrade, P.**; Silva, I.; Silva, M.; Flores, T.; Cassiano, J.; Costa, D.G. *A TinyML Soft-Sensor Approach for Low-Cost Detection and Monitoring of Vehicular Emissions*. SENSORS 2022, 22, 3838.  ![GitHub](https://img.shields.io/badge/DOI-10.3390%2Fs22103838-green)

[[2]](https://www.mdpi.com/1424-8220/21/12/4153) :books: Signoretti, G. ; Silva, M. ; **Andrade, P.**; Silva, I. ; Sisinni, E. ; Ferrari, P.; *An Evolving TinyML Compression Algorithm for IoT Environments Based on Data Eccentricity*. SENSORS 2021, v. 21, p. 4153. ![GitHub](https://img.shields.io/badge/DOI-10.3390%2Fs21124153-green)

[[3]](https://dl.acm.org/journal/tecs) :books: **Andrade, P.**; Silva, I.; Silva, M.; Flores, T.; Costa, D.G. Soares, E.; _Online Processing of Vehicular Data on the Edge Through an Unsupervised TinyML Regression Technique_. ACM TECS 2023. ![GitHub](https://img.shields.io/badge/DOI-under%20review-blue)

# License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

# About us

The research group [**Conect2AI**](http://conect2ai.dca.ufrn.br) consists of undergraduate and graduate students from the Federal University of Rio Grande do Norte (UFRN) and aims to apply Artificial Intelligence (AI) and machine learning in emerging fields. Our expertise includes Embedded Intelligence and IoT, optimizing resource management and energy efficiency, contributing to sustainable cities. In energy transition and mobility, we apply AI to optimize energy use in connected vehicles and promote more sustainable mobility.