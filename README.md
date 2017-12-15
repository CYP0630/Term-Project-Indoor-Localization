# Building/Floor Classification and Location Estimation using WiFi Signals
***
#### **EEE413 Term Project: Indoor localization**
**Professor:** Dr.Kyeong Soo Kim (Joseph)  
**Student:** Yupeng Cao, 1302533

#### Catalogue
* Introduction
* Methodology
* Optimizing Logically
* Results and Discussions 
* Conclusions

## Introduction
### Background
Indoor Localization is a challenging task and there exist no universal solution for all possible applications.

External infrastructure is efficient for localization in limited areas. In large buildings the most precise agent's pose estimates are obtained with laser scanners, however laser scabbers are expensive.

WiFi information can be exploited to provide rough, global position estimates, without additional costs of exteroceptive sensors.

### Related Work
**WiFI Ranging:** the properties of WiFi signal wave are exploited to directly estimate the distance to the access points.

**WiFi Fingerprinting:** Focus on efficiently comparing achieved WiFi scans to the prerecorded database of scans inside building and thus are more robust to local signal disturbances.

**k Nearest Neighbors:** k scans that are the most similar to the analyzed WiFi scan are queried from the database and their positions are averaged to achieve the position estimate.

### Motivation
Those solutions are difficult to tune in a case of a larger building and if a large amount of data is available.

However, the growing amount of available date is caused by the popularity if mobile devices equipped with WiFi adapters.Therefore, machine learning approaches are a promising solution due to less parameter tuning and better scalability in larger environments.GPU processing capabilities improving also can rise the performance.

This project propose DNN approach for floor and building classification and location.

## Methodology
![hey](figure/SAE.png)
The figure shows the SAE Model. 
![Here is SAE Model](figure/Training.png)
The figure shows the Classifier Training Model.

##Optimizing Logically
##Results and Discussions 
![256512accuracy](figure/256512.png)
![binaryaccuracy](figure/binary.png)

##Conclusions

##Reference  
<sup><a id="fn.1" class="footnum" href="#fnr.1">1</a></sup> M. Nowicki and J. Wietrzykowski, "Low-effort place recognition with WiFi fingerprints using deep learning," arXiv:1611.02049v2 [cs.RO] [(arXiv)](https://arxiv.org/abs/1611.02049v2)

<sup><a id="fn.2" class="footnum" href="#fnr.2">2</a></sup> T. Yamashita et al., "Cost-alleviative learning for deep convolutional neural network-based facial part labeling," *IPSJ Transactions on Computer Vision and Applications*, vol. 7, pp. 99-103, 2015. [(DOI)](http://doi.org/10.2197/ipsjtcva.7.99)
