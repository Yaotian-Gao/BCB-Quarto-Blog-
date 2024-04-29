

首先，我需要写一段Preamble。在作业中对该段落的要求如下：

Write a brief paragraph describing the primary question or purpose of the post. Ideally, the concept should be challenging enough that it requires at least two visualizations that use different idioms (ie. don’t just make two scatterplots with different variables). The concept should also be challenging enough that it captures the interest of the reader (i.e. a plot of height and weight that shows they are correlated is trivial and not appropriate). The best approach is to explore a topic or question in which YOU are very interested.

现在，请你针对这一要求，修改以下的Introduction部分，使其符合要求。注意保留参考文献的引用。词数控制在300词左右：

***\*Introduction\****

Wheat (**Triticum aestivum** L.) is one of the most important cereal crops worldwide, providing around 20% of the global caloric intake (Shiferaw et al. 2013). However, both natural and anthropogenic factors are posing significant threats to global food security. An analysis of wheat breeding data in North America from 1960 to 2018 suggests that the current pace of variety improvement may not be sufficient to keep up with the negative impacts of climate change on wheat production (Zhang et al. 2022). Furthermore, the Ukraine-Russia war in 2022 has disrupted one-third of the global wheat exports, which is likely to have severe repercussions on global food security for months, if not years, to come (Bentley et al. 2022). Given these challenges, enhancing wheat yield remains a critical priority in wheat breeding efforts to ensure sustainable food production and global food security.

Yield is a complex trait influenced by multiple factors; therefore, identifying and targeting important yield-related traits is crucial for yield improvement (Isham et al. 2021). Yield components, such as spikelet number per spike and thousand kernel weight, typically show higher heritability than grain yield itself (Wang et al. 2018; Zhang et al. 2018). Plant height is another key trait closely associated with plant architecture, lodging resistance, and yield performance (Wang et al. 2017b). Additionally, heading date can significantly influence wheat adaptability to different environments, thus affecting yield (Chen et al. 2022). Therefore, a comprehensive understanding of yield and yield-related traits and their genetic basis is essential for developing high-yielding wheat varieties through targeted breeding efforts.

Despite the importance of these traits, their phenotypic evaluation can be time-consuming and labor-intensive. Currently, traditional breeding methods, such as hybridization and phenotypic selection, remain essential components of wheat breeding programs (Ahmar et al. 2020a). However, these approaches have several limitations. Firstly, field trials require substantial resources, including land, labor, and time, often taking up to 10-20 years to develop new varieties. Secondly, phenotypic data collection faces challenges such as the need for large-scale manual measurements, potential subjectivity in assessments, and the influence of environmental factors (Ahmar et al. 2020b; Cha et al. 2023). These limitations highlight the need for more efficient and cost-effective approaches to accelerate the wheat breeding process and improve the accuracy of trait evaluation.

The rapid advancement of low-cost, high-throughput genotyping technologies has provided wheat breeders with an abundance of molecular markers spanning the entire genome, facilitating the development of genomic selection (GS) as a promising tool to address the limitations of traditional breeding methods. GS utilizes genome-wide markers to capture the genetic relationships among individuals, enabling the evaluation of complex traits controlled by multiple genes (Zhang et al. 2007). The GS process typically involves a reference population and a breeding population. First, phenotypic and genotypic data from the reference population are used to train a prediction model. Subsequently, the trained model and genotypic data of the breeding population are employed to calculate the genomic estimated breeding values (GEBVs) for the individuals in the breeding population(Larkin et al. 2019). Finally, individuals within the breeding population can be determined using GEBVs, even in the absence of phenotypic information(Xu et al. 2020). Heffner et al. (2009) highlighted that GS has the potential to accelerate breeding cycles, increase genetic gain per unit time, and significantly improve the efficiency of breeding programs by reducing the reliance on extensive phenotyping.

Several factors can influence the prediction accuracy of GS models, including population structure, training population size, and the choice of prediction models (Plavšin et al. 2021). Selecting an appropriate prediction model is a relatively straightforward approach to improve prediction accuracy among these factors. GS models encompass both parametric methods (e.g., Ridge Regression) and non-parametric methods (e.g., Reproducing Kernel Hilbert Space and Random Forest), which differ in their assumptions and handling of marker effects (Desta and Ortiz 2014). In theory, non-parametric methods, which account for non-additive marker effects, should outperform parametric methods. However, the reality is more complex. For instance, Joshi et al. (2024) found that Ridge Regression best explained the variability in the phenotypic expression when predicting test weight in wheat. In another study, Ali et al. (2020) investigated the prediction of grain yield and five other yield-related traits in wheat, including spike number per square meter, thousand kernel weight, spike length, heading date, and plant height. They discovered that the best-performing model varied for each trait. These findings underscore the importance of evaluating and comparing different GS models for specific traits and datasets to identify the most suitable approach. Further research is needed to explore optimal models that maximize prediction ability and computational efficiency across a wide range of traits and datasets.

GS has been successfully applied in wheat breeding for various objectives, including yield improvement, disease resistance, and quality traits, and has even been explored for the domestication of new crops (Rasheed and Xia 2019). However, studies focusing on the application of GS for predicting yield and yield-related traits in wheat, particularly in spring wheat, are still limited. Therefore, further investigations are needed to assess the potential of GS in improving these economically important traits. 

The present study aims to assess the genomic prediction accuracy of different models, including parametric and semi-parametric approaches, in predicting plant height (PHT), total spikelet number per spike (tSNS), heading date (HD), thousand kernel weight (TKW), and yield (YLD) in spring wheat. Six statistical models, namely Ridge Regression (RR), Reproducing Kernel Hilbert Space (RKHS), Genomic Best Linear Unbiased Prediction (GBLUP), Least Absolute Shrinkage and Selection Operator (LASSO), Support Vector Machine (SVM), and Random Forest (RF), were evaluated to identify the optimal model for each trait. The study was conducted using a diverse panel of 250 spring wheat lines, encompassing three market classes (soft white spring, hard white spring, and hard red spring) By leveraging the power of genomic prediction and utilizing a diverse spring wheat population evaluated in multiple environments, this research aims to facilitate precise breeding for improved yield and yield-related traits in spring wheat.



要求：

Data 

Write a summary of the data sources you will use. Include a `Data Dictionary` table that fully describes each individual data file used. You may use your own research data or publicly available data from any source you like (with attribution). There aren’t any minimum or maximum data set size requirements, other than you need something big enough to be interesting and not so big that we don’t have a supercomputer capable of creating your visualization.

相关的资料如下：

Plant Material

This study selected 250 spring wheat varieties and elite lines (Supplemental Table 1). This collection was developed by breeding programs in the Northwestern Pacific region of the United States and the International Maize and Wheat Improvement Center (CIMMYT, Mexico City, Mexico). It encompasses three market categories of spring wheat cultivated in the Americas: soft white spring, hard white spring, and hard red spring, with the majority of the lines (>50%) serving as founding lines for variety development programs in the region.

Phenotypic Evaluation

The panel was evaluated across five environments, designated as E1 to E5, with each year considered a distinct environment (E1 = 2016, E2 = 2017, E3 = 2021, E4 = 2022, E5 = 2023). The field trials were conducted at Aberdeen, Idaho located at 42°56'36" N and 112°50'22" W. The field design was a randomized complete block with two replicates. Each genotype was planted in 3.0 m plots consisting of seven rows, with a row spacing of 21 cm. 

Yield per acre (YLD) in kilograms per hectare (kg/ha) was evaluated in four trials (E1, E2, E4, E5).

Genotyping

The population was genotyped using Illumina's 90K iSelect SNPchip. Raw data was provided by the USDA/ARS Cereal Crops Research Unit and was analyzed using Genome Studio v2.0.5(Illumina 2010) for processing its raw data. Polymorphic markers were identified as exhibiting clear, distinct clusters in Genome Studio, with a minimum distance of 0.20 between the polar coordinates of normalized theta intensities. Markers were further filtered based on missing data (>10%) and minor allele frequency (<5%) using TASSEL v5.2.89 (Bradbury et al. 2007).

我的文件储存在YLD.csv文件中

另外，这是一个.qmd文件。请问要求中的`Data Dictionary` table 是不是需要特殊设置呢？



### Data Dictionary

| Field     | Description                                                  | Data Type |
| --------- | ------------------------------------------------------------ | --------- |
| ENT       | Unique identifier for each wheat variety, numbered from 52001 to 52250 | Integer   |
| Source    | Source of the plant material, including universities (UI, UCD, WSU), CIMMYT, MSU, USDA, and other sources (commercial varieties and international germplasm) | String    |
| YLD_E1    | Yield in kilograms per hectare for environment E1 (2016)     | Float     |
| YLD_E2    | Yield in kilograms per hectare for environment E2 (2017)     | Float     |
| YLD_E4    | Yield in kilograms per hectare for environment E4 (2022)     | Float     |
| YLD_E5    | Yield in kilograms per hectare for environment E5 (2023)     | Float     |
| YLD_BLUPs | Best Linear Unbiased Prediction (BLUP) values for yield, calculated from the yields of environments E1, E2, E4, and E5. NA indicates not applicable. | Float     |



| Df   | Sum Sq      | Mean Sq     | F value     | Pr(>F)   | R^2^  |
| ---- | ----------- | ----------- | ----------- | -------- | ----- |
| 6    | 1383462.467 | 230577.0778 | 5.068379905 | 6.41E-05 | 11.1% |
| 242  | 11009366.68 | 45493.25073 | NA          |          |       |

| Trait | Env   | Mean     | Range                    | IQR      | CV    | Skewness | Kurtosis |
| ----- | ----- | -------- | ------------------------ | -------- | ----- | -------- | -------- |
| YLD   | E1    | 5687.207 | 3560.188-7753.867±839.68 | 1115.165 | 0.148 | -0.258   | -0.285   |
|       | E2    | 5528.63  | 4850.76-6181.51±272.1    | 356.24   | 0.05  | -0.18    | -0.22    |
|       | E4    | 6012.449 | 5512.441-6517.149±178.2  | 216.375  | 0.03  | -0.017   | 0.31     |
|       | E5    | 6630.67  | 5603.001-7432.273±327.87 | 428.973  | 0.049 | -0.243   | -0.11    |
|       | BLUPs | 6023.156 | 5340.134-6550.368±223.86 | 290.7    | 0.037 | -0.292   | -0.122   |

| Traits | Training Environments | Prediction Environments | Prediction accuracies a |
| ------ | --------------------- | ----------------------- | ----------------------- |
| YLD    | BLUPs                 | BLUPs                   | 0.424                   |
|        |                       | E1                      | 0.369                   |
|        |                       | E2                      | 0.325                   |
|        |                       | E4                      | 0.189                   |
|        |                       | E5                      | 0.240                   |
| YLD    | E1                    | BLUPs                   | 0.288                   |
|        |                       | E1                      | 0.565                   |
|        |                       | E2                      | 0.277                   |
|        |                       | E4                      | 0.109                   |
|        |                       | E5                      | -0.052                  |
| YLD    | E2                    | BLUPs                   | 0.319                   |
|        |                       | E1                      | 0.343                   |
|        |                       | E2                      | 0.360                   |
|        |                       | E4                      | 0.140                   |
|        |                       | E5                      | 0.041                   |
| YLD    | E4                    | BLUPs                   | 0.161                   |
|        |                       | E1                      | 0.242                   |
|        |                       | E2                      | 0.129                   |
|        |                       | E4                      | 0.078                   |
|        |                       | E5                      | 0.058                   |
| YLD    | E5                    | BLUPs                   | 0.259                   |
|        |                       | E1                      | 0.024                   |
|        |                       | E2                      | 0.053                   |
|        |                       | E4                      | 0.127                   |
|        |                       | E5                      | 0.395                   |