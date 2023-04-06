# Cole McCall

Hello, my name is Cole McCall, and I am currently seeking an entry-level role in software development or data science, preferably with an emphasis in GIS.

I graduate from Northwest Nazarene University in May 2023 with a major in Computer Science and concentrations in Data Science and Cyber Security. While attending NNU, my passion for working with software, data, and maps has continued to grow, with classes like Artificial Intelligence, Machine Learning, and Big Data Management challenging me to learn more and apply my absolute best efforts and abilities.

Outside of the classroom, I have worked as a research assistant for over 2 years, where I have worked with my team to use drone and satellite imagery to solve geospatial problems, such as mapping and predicting wildfires, using AI and Machine Learning. Additionally, I have provided help to fellow students and my professors as a teacher’s assistant, where I learned just how true it is that you don’t always know something until you teach it to others.


# Projects
Ever since I began programming, I have discovered that I am someone that learns through doing, not just by watching and observing. As such, I have completed several projects during my college education, along with personal side projects and research projects that I have enjoyed. I have chosen to share a few of these projects here below.

## Artificial Intelligence
During the Spring 2021 semester, I signed up for NNU's COMP4220 Artificial Intelligence as a Sophomore Computer Science student. This was an amazing class for me, as I was really pushed, both conceptually and technically. Throughout the course, I developed programs in C++ that used AI, several of which can be seen down below. While these projects started as homework assignments, they quickly progressed into fun challenges that I wanted to solve and take above and beyond.

### Playing Connect Four with AI
**Project Description:**

**Code:** [https://github.com/colemccall/Connect_Four](https://github.com/colemccall/Connect_Four)


### Cracking the Code with Genetic Algorithms
**Project Description:**

**Code:** [https://github.com/colemccall/Genetic_Algorithm_Cipher_Buster](https://github.com/colemccall/Genetic_Algorithm_Cipher_Buster)


### Finding the Best Path on a Map
**Project Description:**

**Code:** [https://github.com/colemccall/Pathfinder](https://github.com/colemccall/Pathfinder)


## General Education Data Science
**Project Description:** During my Senior year, I started in a project in the Advanced Database Management course, which turned in a part-time project that I am still consulting/advising on. Based on course and student data stored in spreadsheets, our team of 3 was tasked with cleaning, storing, and finding patterns in the data, which was used to provide insights into which general education courses are being properly assessed, and how to predict this information in the future.

**Code:** [https://github.com/colemccall/NNU_Gen_Ed_Data_Science](https://github.com/colemccall/NNU_Gen_Ed_Data_Science)


## Computer Vision for Rocksat-X 2022
**Project Description:** Object detection with a MaskR-CNN

**Code:** [https://github.com/colemccall/RockSatX2022_Object_Detection](https://github.com/colemccall/RockSatX2022_Object_Detection)


# Research
Over the past few years, the size and severity of wildland forest fires have continued to increase, causing more damage and destruction around the world. New methods have been developed to utilize machine learning algorithms to map forest fire burn extent and fire severity using aerial imagery. Algorithms such as the Support Vector Machine (SVM) can be used to classify pixels as either black ash, white ash, or unburned, while the Mask Region-Based Convolutional Neural Network (MaskR-CNN) can be used to find and map tree objects. The results from these classifications can be used to help local wildland fire managers assess the burned area and create a recovery plan.
 
This research has several steps: 1) improving the current method for mapping burn extent with hyperspatial drone imagery, 2) using the same (or similar) methods to determine if wildland fire burn extent can be mapped with high-resolution satellite imagery, 3) evaluating how spatial and spectral resolution impacts the accuracy of the classification, and 4) try to develop new methods that involve less (or no) training data, such as unsupervised change detection. The results of each step were promising, creating much more accurate classifications of wildland fire burn extent than can be obtained by other common products such as LANDFIRE. This research will continue, likely moving in a direction that further examines the use of unsupervised and self-supervised machine learning, which greatly reduces the training data needed.


## Mapping Wildfires with Drone Imagery using Machine Learning
**Project Description:** 
Based on previous research, machine learning algorithms such as the Support Vector Machine (SVM) have been used to accurately map the burn extent of wildland fires, whereas a Mask Region-Based Convolutional Neural Network (Mask R-CNN) could be used to detect tree objects. Since surface vegetation on the ground may be obstructed by tree crowns above, the aerial imagery captured by drones may produce an inaccurate mapping of the burn extent, observing the tree crown on top instead of the possibly burned vegetation underneath. To enhance the burn extent classification, a program was developed to find all tree objects completely surrounded by burned areas and reclassify those tree objects as burned regions since the areas underneath the tree crown were burned, even though the tree crown itself did not burn. 


**INSERT IMAGES FROM SLIDES**


The results of this project were published in an article in the Remote Sensing journal titled “Mapping Forest Burn Extent from Hyperspatial Imagery Using Machine Learning”, which is available to read [here](https://www.mdpi.com/2072-4292/13/19/3843)


**Responsibilties/Impact:**


## Evaluating the Impacts of Spatial and Spectral Resolutions in using Satellite Imagery for Classification
**Project Description:** 

Even though hyperspatial drone imagery can accurately map burn extent, it can be difficult and time-consuming to collect/acquire drone imagery. Additionally, mapping the burn extent involves utilizing an SVM classifier that must be trained to the image, a MaskR-CNN that must be trained to detect trees, and an additional program to enhance the burn extent created by the SVM classifier. For these reasons, the FireMAP research team began to study how substituting 5cm spatial resolution drone imagery for lower 1.5 to 3m spatial resolution satellite imagery affected the accuracy of mapping burn extent. While this high-resolution satellite imagery has a lower spatial resolution (~1.5 to 3m instead of 5cm), the satellite imagery has a higher spectral resolution, containing eight multispectral bands as opposed to the typical Red, Green, and Blue (RGB) bands of an image. When using satellite imagery instead of drone imagery, the higher spatial resolution is swapped for a higher spectral resolution, introducing bands like Red Edge, Yellow, and Near Infrared into the mix. 

The changes in resolution between images created another aspect to this research: evaluating how spatial resolution and spectral band selection impact the accuracy of a burn extent classification. Two sets of satellite imagery were used to explore these ideas: ~1.8m spatial resolution Worldview2 imagery and ~3m spatial resolution PlanetScope imagery. 

**INSERT IMAGES COMPARING PRODUCTS FROM SLIDES**

A manuscript is currently being developed for evaluating spatial resolution and spectral band selection with Worldview2 imagery. 

A separate manuscript for mapping burn extent from PlanetScope imagery is expected to begin development this summer.


**Responsibilties/Impact:**


## Unsupervised Wildfire Change Detection
**Project Description:**
 In the summer of 2022, NNU’s summer research team assisted in the FDL-US 2022 Wildfire Challenge, at Frontier Development Lab (FDL). The wildfire research team was given a challenge by the U.S. Department of Energy to determine if “... ML-enhanced tools can be used to prevent fires from starting or new fires from combining to create mega-fires". The FDL-US 2022 Wildfire team wanted to use machine learning algorithms to map burn extent from satellite imagery. However, this team wanted to use self-supervised learning instead of supervised learning methods that require large amounts of training data. 
 
 Additionally, the wildfire team partnered with Planet, who gave the team access to ~3m spatial resolution PlanetScope imagery, with near-daily updates, which gave the team even more opportunities. This project aimed to use the PlanetScope imagery to perform daily wildfire change detection, which could then be used to predict wildfire changes in simulation. An advanced deep learning technique called contrastive learning was used to perform unsupervised change detection, which resulted in detecting burn area change. The results of this project were published in “Unsupervised Wildfire Change Detection based on Contrastive Learning”, which can be found [here](https://arxiv.org/abs/2211.14654)


 **Responsibilties/Impact:**



# Links
- [LinkedIn](https://www.linkedin.com/in/colemccall/)
- [GitHub](https://github.com/colemccall)
- [Resume](Cole%20McCall%20April%202023%20Resume.pdf)