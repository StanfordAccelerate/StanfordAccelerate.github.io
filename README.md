# People
## Faculty

| | Priyanka Raina |
|:-------------|:------------------|
| Email            | praina@stanford.edu |
| Contact          | Allen Building - Room 114, (617) 899-3791 |
| About            | Priyanka Raina is an Assistant Professor in Electrical Engineering at Stanford University. Previously, she was a Visiting Research Scientist in the Architecture Research Group at NVIDIA Corporation. She received her Ph.D. degree in 2018 and S.M. degree in 2013 in EECS from MIT and her B.Tech. degree in EE from IIT Delhi in 2011. |
| Research Summary | |

## Adminitrator

| | Julie Kline |
|:-------------|:------------------|
| Email            | klinej@stanford.edu |
| Contact          | Packard Building - Room 359, (650) 723-4539 |


## Students
### PhD Students

|              | Haitong Li            |
|:-------------|:----------------------|
| Email        | haitongl@stanford.edu |
| Webpage      | |
| About        | |
| Research     | |

|              | Weier Wan             |
|:-------------|:----------------------|
| Email        | weierwan@stanford.edu |
| Webpage      | |
| About        | |
| Research     | |

### PhD Rotation Students

|              | Akash Levy           |
|:-------------|:----------------------|
| Email        | akashl@stanford.edu |
| Webpage      | |
| About        | |
| Research     | |

|              | Fei Huang             |
|:-------------|:----------------------|
| Email        | feihuang@stanford.edu |
| Webpage      | |
| About        | |
| Research     | |

### Masters Students

|              | Kartik Prabhu         |
|:-------------|:----------------------|
| Email        | kprabhu7@stanford.edu |
| Webpage      | |
| About        | |
| Research     | |

## Previous Students
### PhD Rotation Students

|              | Raman Vilkhu          |
|:-------------|:----------------------|
| Email        | vilkhu@stanford.edu |
| Webpage      | |
| About        | |
| Research     | |

# Research
## Current Projects

### Agile Hardware (AHA)
**Faculty: Priyanka Raina, Mark Horowitz, Pat Hanrahan, Clark Barrett, Kayvon Fatahalian**

(Webpage)[https://aha.stanford.edu], (Github)[https://github.com/StanfordAHA]

#### Peak

#### Gemstone

#### Whitney

#### Garnet: The second generation Coarse Grained Reconfigurable Array (CGRA) Architecture optimized for neural networks and image processing applications

#### SoC
* ARM Based
* RISC-V Based

* * *

### In-Memory Compute Architecture for One-Shot Learning Applications

**People: Haitong Li, Philip Wong, Priyanka Raina**

* * *

### Hybrid RRAM/NEMS-Based 3D Interconnect Design for Programmable Logic Devices

**People: Akash Levy, Priyanka Raina**

* * *

### Emerging Non Volatile Memory - Centric Accelerator for Deep Neural Network Inference and Training in 5G Applications

**People: Fei Huang, John Cioffi, Priyanka Raina**

* * *

### NVM-Based Neural Network Accelerators

**People: Fei Huang, Daniel Bankman, Robert M. Radway, Jonas Messner, Kartik Prabhu, Binh Q. Le, Priyanka Raina, Subhasish Mitra, Boris Murmann**

* * *

### RBM Accelerator

**People: Weier Wan, ...**

* * *

### DNN Accelerator Generator

** People: Kartik Prabhu, Xuan Yang, Mark Horowitz, Priyanka Raina **

* * * 

## Upcoming Projects

### Optimizing Computer Vision Performance with Energy-Efficient Deep ISPs
**People: Gordon Wetzstein, Priyanka Raina**

**We are looking for graduate students to work on this project! Please email Priyanka if you are interested.**

The capacity of imaging systems must continue to expand in order to keep pace with rapidly increasing, application-specific demands in robotic and machine vision, consumer photography, autonomous driving, surveillance and machine learning. State-of-the-art imaging systems optimize the image processing pipeline (ISP) for image quality as perceived by a human observer and they treat different stages of the ISP as separate blocks, which leads to sub-optimal performance. In particular, sensor noise, defocus and motion blur, as well as other imperfections in the image formation, especially in low-light environments, are fundamental challenges for achieving state of the art performance of computer vision algorithms, such as image classification and object detection with current ISPs. 

Stanford Computational Imaging Lab has proposed an optimization-based ISP approach that outperforms commercial implementations of Google Nexus phones significantly. They have recently explored novel end-to-end differentiable architecture for joint denoising, deblurring, and image classification that makes classification robust to realistic noise and blur. This architecture dramatically improves the accuracy of a classification network in low light and other challenging conditions, outperforming alternative approaches such as retraining the network on noisy and blurry images and preprocessing raw sensor inputs with conventional denoising and deblurring algorithms. The architecture learns denoising and deblurring pipelines optimized for classification whose outputs differ markedly from those of state-of-the-art denoising and deblurring methods, preserving fine detail at the cost of more noise and artifacts. These results suggest that the best low-level image processing for computer vision is different from existing algorithms designed to produce visually pleasing images.

At the same time, we recognize that the algorithms for computational imaging and vision are rapidly evolving, and hardware must follow suit: the next generation of hardware ISPs must be "programmable" to support new algorithms created with high-level frameworks. Our results for the AHA project suggest that the best programmable ISPs would be heterogeneous CGRAs with a multitude of small ASIC-style compute units. In this project, we will design an end-to-end ISP pipeline for computer vision tasks, primarily focusing on the application of object detection. Moreover, we will explore deep neural network architectures that generalize across other applications, including segmentation, tracking, face detection, and more. A dedicated neural network will be trained for all of these applications separately, but the larger goal of this project is to develop a unifying network architecture that represents the state-of-the-art computer vision pipeline (optimizing high-level vision tasks). We will also create a CGRA hardware architecture (and its programming toolchain) with compute units optimized for running this unifying network at high performance and energy-efficiency. We expect the outcome of this project to lay the foundations of future energy-efficient and programmable mobile image processors.

* * *

### Objective Body Surface Area Determination for the Investigation of Vitiligo Clinical Outcomes
**People: Dr. Victor Huang (UC Davis), Priyanka Raina**

**We are looking for students to work on this project! Please email Priyanka if you are interested.**

Vitiligo is an autoimmune condition that targets melanocytes, the pigment producing cells of the skin, and results in large patches of skin losing their color. It affects approximately 1% of the population and has significant negative effects on the quality of life of patients. Vitiligo progresses over the course of months to years and response to treatment may, similarly, require months to years to become apparent. This is a significant hurdle as selecting an optimal treatment strategy such as immune suppression versus surgical approaches hinges on being able to accurately assess residual disease activity. However, there is no sensitive and objective outcome measure to characterize the spread of the disease, and this has been a major hurdle for optimizing clinical care as well as for development of clinical trials for vitiligo.

To assess the spread of vitiligo, a clinician commonly performs a visual examination of the patient and assigns a VASI (Vitiligo Area Scoring Index), or a VETF (Vitiligo European Task Force) score that corresponds to the depigmented body surface area (BSA) or ‘lesion(s)’. However, this method has low accuracy, high variability, and is insensitive to small changes. The gold standard of lesion area assessment involves planimetry, where a lesion is manually traced onto a transparent grid sheet from which area is calculated. This approach is time intensive, however, and limited to individual lesions and not suited to evaluating involvement across an entire body or region. There have been attempts at measuring relative change in lesion area using image analysis based on 2D color images which do not require manual lesion segmentation but they still introduce a 20-40% error in area calculated depending on the angle of image acquisition since the lesions are on curved body surfaces. Additionally, they only measure relative area change between two images taken at different times, and not absolute surface area.

We propose the development and clinical evaluation of a fully-automated computer-assisted system that quantitatively and accurately assesses 3D BSA using depth and color imaging and machine learning based vision algorithms. The greater sensitivity of this method will detect currently sub- clinical changes, which can be clinically significant in defining disease activity and predicting both initial response and durability of response to treatment. In addition, this technology can be later adapted for analysis of any skin condition for which BSA is an outcome measure of interest, such as psoriasis, melanoma, dermatological reactions to drugs and wounds.
