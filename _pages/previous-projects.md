---
permalink: /previous-projects/
toc: true
---
## Previous Projects

### A Scalable Multi-Chip-Module-based DNN Accelerator Designed with a High-Productivity VLSI Methodology
![](/assets/images/simba.png){: .align-right .width-fifty-percent}

In this work, a scalable deep neural network (DNN) inference accelerator consisting of 36 small chips connected in a mesh network on a multi-chip-module (MCM) was designed. The accelerator enables flexible scaling for efficient inference on a wide range of DNNs, from mobile to data center domains. The chip was implemented using a novel high-productivity VLSI methodology, fully designed in C++ using High-Level Synthesis (HLS) tools and leveraged an agile VLSI design flow. The 6 mm2 chip was implemented in 16nm technology and achieves 1.29 TOPS/mm2, 0.11 pJ/op energy efficiency, 4 TOPS peak performance on 1 chip, and 128 peak TOPS and 2,615 images/s ResNet-50 inference in a 36-chip MCM.

**Publications:**

**A 0.32-128 TOPS, Scalable Multi-Chip-Module-based Deep Neural Network Inference Accelerator with Ground-Referenced Signaling in 16nm**  
B. Zimmer, R. Venkatesan, S. Shao, J. Clemons, M. Fojtik, N. Jiang, B. Keller, A. Klinefelter, N. Pinckney, P. Raina, S. G. Tell, Y. Zhang, W. J. Dally, J. S. Emer, C. T. Gray, S. W. Keckler, B. Khailany  
*Journal of Solid-State Circuits (JSSC)*, January 2020. [Paper](https://ieeexplore.ieee.org/document/8959403)

**MAGNet: A Modular Accelerator Generator for Neural Networks**  
R. Venkatesan, S. Shao, M. Wang, J. Clemons, S. Dai, M. Fojtik, B. Keller, A. Klinefelter, N. Pinckney, P. Raina, Y. Zhang, B. Zimmer, B. Dally, J. Emer, S. Keckler, B. Khailany  
*International Conference On Computer Aided Design (ICCAD)*, November 2019. [Paper](https://pdfs.semanticscholar.org/f9b9/90566338411ca302787687a5d0c5dc68b692.pdf?_ga=2.50549674.287759541.1574145941-1788187331.1574145941)

**Simba: Scaling Deep-Learning Inference with Multi-Chip-Module-Based Architecture**  
S. Shao, J. Clemons, R. Venkatesan, B. Zimmer, M. Fojtik, N. Jiang, B. Keller, A. Klinefelter, N. Pinckney, P. Raina, S. Tell, Y. Zhang, B. Dally, J. Emer, C. T. Gray, B. Khailany, S. Keckler  
*International Symposium on Microarchitecture (MICRO)*, October 2019. **([Best Paper Award](https://www.microarch.org/micro52/program/bestpaper.html), Top Picks in Computer Architecture Honorable Mentions)** [Paper](https://people.eecs.berkeley.edu/~ysshao/assets/papers/shao2019-micro.pdf)

**A 0.11 pJ/Op, 0.32-128 TOPS, Scalable Multi-Chip-Module-based Deep Neural Network Accelerator Designed with a High-Productivity VLSI Methodology**  
B. Khailany, R. Venkatesan, Y. S. Shao, B. Zimmer, J. Clemons, M. Fojtik, N. Jiang, B. Keller, A. Klinefelter, N. Pinckney, P. Raina, S. G. Tell, Y. Zhang, W. J. Dally, J. S. Emer, C. T. Gray, S. W. Keckler  
*Hot Chips: A Symposium on High Performance Chips (HotChips)*, August 2019. [Slides](https://people.eecs.berkeley.edu/~ysshao/assets/papers/venkatesan2019-hotchips.pdf)

**A 0.11 pJ/Op, 0.32-128 TOPS, Scalable Multi-Chip-Module-based Deep Neural Network Accelerator with Ground-Reference Signaling in 16nm**  
B. Zimmer, R. Venkatesan, Y. S. Shao, J. Clemons, M. Fojtik, N. Jiang, B. Keller, A. Klinefelter, N. Pinckney, P. Raina, S. G. Tell, Y. Zhang, W. J. Dally, J. S. Emer, C. T. Gray, S. W. Keckler, B. Khailany  
*Symposium on VLSI Circuits (VLSI)*, June 2019. [Paper](https://ieeexplore.ieee.org/document/8778056)

* * *

### Automating Vitiligo Skin Lesion Segmentation Using Convolutional Neural Networks
![](/assets/images/vitiligo.jpg){: .align-right .width-eighty-percent}

The measurement of several skin conditions' progression and severity relies on the accurate segmentation (border detection) of lesioned skin images. One such condition is vitiligo. Existing methods for vitiligo image segmentation require manual intervention, which is time and labor-intensive, as well as irreproducible between physicians. We introduce a convolutional neural network (CNN) that quickly and robustly performs such segmentations without manual intervention. We use the U-Net with a modified contracting path to generate an initial segmentation of the lesion. Then, we run the segmentation through the watershed algorithm using high-confidence pixels as “seeds.” We train the network on 247 images with a variety of lesion sizes, complexities, and anatomical sites. Our network noticeably outperforms the state-of-the-art U-Net - scoring a Jaccard Index (JI) of 73.6% (compared to 36.7%). Segmentation occurs in a few seconds, which is a substantial improvement from the previously proposed semiautonomous watershed approach (2–29 minutes per image).

**Publications:**

**Automating Vitiligo Skin Lesion Segmentation Using Convolutional Neural Networks**  
M. Low, V. Huang, P. Raina  
*IEEE International Symposium on Biomedical Imaging (ISBI)*, April 2020. [Paper](https://ieeexplore.ieee.org/abstract/document/9098682)

* * *

### Timeloop: A Systematic Approach to DNN Accelerator Evaluation

Timeloop is an infrastructure for evaluating and exploring the architecture design space of deep neural network (DNN) accelerators. Timeloop uses a concise and unified representation of the key architecture and implementation attributes of DNN accelerators to describe a broad space of hardware topologies. It can then emulate those topologies to generate an accurate projection of performance and energy efficiency for a DNN workload through a mapper that finds the best way to schedule operations and stage data on the specified architecture. This enables fair comparisons across different architectures and makes DNN accelerator design more systematic. 

**Publications:**

**Timeloop: A Systematic Approach to DNN Accelerator Evaluation**  
A. Parashar, P. Raina, S. Shao, A. Mukkara, V. A. Ying, R. Venkatesan, Y. H. Chen, B. Khailany, S. Keckler, J. Emer  
*International Symposium on Performance Analysis of Systems and Software (ISPASS)*, March 2019. [Paper](https://ieeexplore.ieee.org/document/8695666)

**Code:**  
[https://github.com/NVlabs/timeloop](https://github.com/NVlabs/timeloop)

* * * 

### A Low-Power Accelerator for Real-Time Motion Magnification in Videos

![](/assets/images/motion_chip.png){: .width-seventy-percent}

Many phenomena around us exhibit small motions that are invisible to the naked eye. Recent research has shown that computational amplification can be used to reveal such motions. However, state of the art motion magnification algorithms are computationally intensive and achieve a throughput of only 0.23 frames/s while consuming 10.36μJ energy/pixel on mobile CPUs for FullHD video, which is 4 orders of magnitude higher than what is required for their energy-efficient mobile implementation. This work presents the first low-power accelerator for motion magnification that achieves real-time performance on FullHD video at 30 frames/s, while consuming only around 10nJ of energy/pixel. The processor accelerates the motion magnification algorithm using a Riesz pyramid to decompose each frame of the input video and separate the amplitude of the local wavelets from their phase. It then performs temporal filtering of the phases independently at each location, orientation and scale to isolate the frequencies of interest (for example, a band around 1 Hz for breathing rate amplification). This is followed by spatial smoothing to reduce noise in the phase, and finally amplification and reconstruction of the output video by inverting the pyramid. We use several techniques in the design of the accelerator to achieve energy-efficiency and real-time performance: (1) separable filtering with reordering in Riesz pyramid computation to reduce the number of multiplies by 5.25x and number of adds by 3x, and zero-skipping to reduce pyramid buffering size by 23.3%, (2) compressing the computed Riesz pyramid data to reduce memory bandwidth and save system energy, (3) detecting active pixels, which are typically less than 50% of total pixels, from the temporal filter output, and performing motion magnification for the subsequent frames on the active pixels only to reduce the amount of computation, memory bandwidth and energy. As a result, the accelerator achieves 130x improvement in performance and 1036x improvement in energy-efficiency over mobile CPUs, enabling, for the first time, efficient integration of motion magnification technology into mobile devices.

* * * 

### An Energy-Scalable Accelerator for Blind Image Deblurring

![](/assets/images/deblur_chip.jpg){: .width-seventy-percent}

Camera shake is the leading cause of blur in cell-phone camera images. Removing blur requires deconvolving the blurred image with a kernel which is typically unknown and needs to be estimated from the blurred image. This kernel estimation is computationally intensive and takes several minutes on a CPU which makes it unsuitable for mobile devices. This work presents the first hardware accelerator for kernel estimation for image deblurring applications. Our approach, using a multi-resolution IRLS deconvolution engine with DFT-based matrix multiplication, a high-throughput image correlator and a high-speed selective update based gradient projection solver, achieves a 78x reduction in kernel estimation runtime, and a 56x reduction in total deblurring time for a 1920 x 1080 image enabling quick feedback to the user. Configurability in kernel size and number of iterations gives up to 10x energy scalability, allowing the system to trade-off runtime with image quality. The test chip, fabricated in 40nm CMOS, consumes 105mJ for kernel estimation running at 83MHz and 0.9V, making it suitable for integration into mobile devices.

**Publications and Talks:**

**An Energy-Scalable Accelerator for Blind Image Deblurring**  
P. Raina, M. Tikekar, and A. P. Chandrakasan  
*Journal of Solid-State Circuits (JSSC)*, July 2017. (Invited) [Paper](https://ieeexplore.ieee.org/document/7891902)

**An Energy-Scalable Accelerator for Blind Image Deblurring**  
P. Raina, M. Tikekar, and A. P. Chandrakasan  
*European Solid-State Circuits Conference (ESSCIRC)*, September 2016. (**Best Young Scientist Paper Award**) [Paper](https://ieeexplore.ieee.org/document/7598255)

**An Energy-Scalable Co-processor for Blind Image Deblurring**  
P. Raina, M. Tikekar, A. P. Chandrakasan  
International Solid-State Circuits Conference (ISSCC) Student Research Preview (SRP) Poster Session, February 2016. (**2016 ISSCC Student Research Preview Award**)

* * *

### Maxwell: A Reconfigurable Processor for Computational Photography

![](/assets/images/hdr_chip.png){: .width-seventy-percent}

Computational photography refers to a wide range of image capture and processing techniques that extend the capabilities of digital photography and allow users to take photographs that could not have been taken by a traditional camera. Since its inception less than a decade ago, the field today encompasses a wide range of techniques including high dynamic range (HDR) imaging, low light enhancement, panorama stitching, image deblurring and light field photography. These techniques have so far been software based, which leads to high energy consumption and typically no support for real-time processing. This work focuses on a hardware accelerator for bilateral filtering which is commonly used in computational photography applications. Specifically, the 40 nm CMOS test chip performs HDR imaging, low light enhancement and glare reduction while operating from 98 MHz at 0.9 V to 25 MHz at 0.9 V. It processes 13 megapixels/s while consuming 17.8 mW at 98 MHz and 0.9 V, achieving significant energy reduction compared to previous CPU/GPU implementations, enabling real-time computational photography applications on mobile devices.

**Publications and Talks:**

**Reconfigurable Processor for Energy-Efficient Computational Photography**  
R. Rithe, P. Raina, N. Ickes, S. V. Tenneti, A. P. Chandrakasan  
*Journal of Solid-State Circuits (JSSC)*, November 2013. [Paper](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=6623206)

**Reconfigurable Processor for Energy-Scalable Computational Photography**  
R. Rithe, P. Raina, N. Ickes, S. V. Tenneti, A. P. Chandrakasan  
*International Solid-State Circuits Conference (ISSCC)*, February 2013. [Paper](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=6487683), [Demo](http://player.vimeo.com/video/70417371)

**In the News:**

* Picture Perfect: Quick, efficient chip cleans up common flaws in amateur photographs. ([MIT News](http://web.mit.edu/newsoffice/2013/computational-photography-chip-0219.html))
* Image Processor Makes for Better Photos and Performance ([IEEE The Institute](http://theinstitute.ieee.org/technology-focus/technology-topic/image-processor-makes-for-better-photos-and-performance))
* MIT imaging chip creates natural-looking flash photos. ([Engadget](http://www.engadget.com/2013/02/21/mit-imaging-chip-blends-shots-with-and-without-flash/))
* MIT's new chip promises 'professional-looking' photos on your smartphone. ([DPReview](http://connect.dpreview.com/post/2110851336/mit-photo-chip-smartphone-photos))
* Improve your smartphone's photo quality with this chip. ([Mashable](http://mashable.com/2013/02/21/photo-chip/))

* * * 

### A 3D Vision Processor for a Navigation Device for the Visually Challenged

![image-left](/assets/images/vision_chip.jpg){: .align-left .width-fifty-percent}

3D imaging devices, such as stereo and time-of-flight (ToF) cameras, measure distances to the observed points and generate a depth image where each pixel represents a distance to the corresponding location. The depth image can be converted into a 3D point cloud using simple linear operations. This spatial information provides detailed understanding of the environment and is currently employed in a wide range of applications such as human motion capture. However, its distinct characteristics from conventional color images necessitate different approaches to efficiently extract useful information. This chip is a low-power vision processor for processing such 3D image data. The processor achieves high energy-efficiency through a parallelized reconfigurable architecture and hardware-oriented algorithmic optimizations. The processor will be used as a part of a navigation device for the visually impaired. This handheld or body-worn device is designed to detect safe areas and obstacles and provide feedback to a user. We employ a ToF camera as the main sensor in this system since it has a small form factor and requires relatively low computational complexity.

**Publications and Talks:**

**A 0.6V 8mW 3D Vision Processor for a Navigation Device for the Visually Impaired**  
D. Jeon, N. Ickes, P. Raina, H. C. Wang, A. P. Chandrakasan  
*International Solid-State Circuits Conference (ISSCC)*, February 2016. [Paper](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=7418084)

**In the News:**

* A virtual “guide dog” for navigation. ([MIT News](http://news.mit.edu/2016/virtual-guide-dog-wearable-device-0202#.VrHZj9k0f5g))
* MIT researchers have developed a ‘virtual guide dog’. ([boston.com](https://www.boston.com/news/local-news/2016/02/03/mit-researchers-have-developed-a-virtual-guide-dog))
* Wearable with 3D camera to guide visually impaired. ([Pune Mirror](http://www.punemirror.in/others/scitech/Wearable-with-3D-camera-to-guide-visually-impaired/articleshow/50855649.cms))

* * *

More details about Priyanka's PhD work are on [Priyanka's MIT webpage](http://web.mit.edu/~praina/www/index.html).
