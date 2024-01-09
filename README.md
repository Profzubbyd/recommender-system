# Recommender System for In-Vehicle Coupon Data

## I. Introduction
Sales are crucial for businesses, and coupons play a significant role in achieving sales goals. This project focuses on building a recommender system for in-vehicle coupon data, aiming to enhance consumer engagement and increase sales. The approach involves collecting survey data through questionnaires, analyzing it using machine learning tools, and gaining insights into consumer behavior to optimize coupon creation.

## II. Related Work
The project draws inspiration from various recommender system literatures, combining deep learning with collaborative filtering, fuzzy expert systems, and hybrid models. Previous works explored applications in smartphone recommendations, online shopping, radio channel recommendations, and in-vehicle coupon systems. Bayesian rule set models and machine learning techniques have been employed to understand customer responses and predict acceptance.

## III. Datasets
The project utilizes the in-vehicle coupon recommendation dataset with 12,684 instances across 26 attributes. Collected through a survey on Amazon Mechanical Turk, the dataset includes information on driving scenarios, demographic details, and coupon acceptance indicators. It can be found in: https://archive.ics.uci.edu/ml/datasets/in-vehicle+coupon+recommendation. The classification goal is to predict whether a person would accept a coupon under specific conditions.

## IV. Methods
The chosen method involves preprocessing the data by transforming categorical attributes into numerical ones, imputing missing values, and normalizing the dataset. The suggested improvements include using classification and regression trees (cart) imputation and predictive mean matching (pmm) imputation for missing values. Additionally, training Extra Trees Classifier, Nu Support Vector Classification (NuSVC), and Light GBM (LGBM) classifiers is recommended.

## V. Experiments
The experiments focus on evaluating the performance of classifiers, including Extra Trees Classifier, NuSVC, and LGBM, using different missing value imputation methods. Results indicate varying accuracy levels (74-77%) with Extra Trees Classifier achieving the highest accuracy. Computation times reveal LGBM as the fastest model. Confusion matrices provide insights into classifier performance.

<p align="center">
  <img width="400" alt="image" src="https://github.com/Profzubbyd/recommender-system/assets/46527701/e3a53700-38ef-400b-964a-2637e2050ad5">
</p>

<p align="center">
    Figure 1: LGBM Classifier confusion matrix
</p>

<p align="center">
  <img width="400" alt="image" src="https://github.com/Profzubbyd/recommender-system/assets/46527701/63c87e1d-1f89-455c-908a-dca67e4105af">
</p>

<p align="center">
  Figure 2: Extra Trees Classifier Confusion Matrix
</p>

<p align="center">
  <img width="400" alt="image" src="https://github.com/Profzubbyd/recommender-system/assets/46527701/210c7a34-0de0-4b55-9538-303ce9b69e2b">
</p>

<p align="center">
  Figure 3: NuSVC Confusion Matrix
</p>

<p align="center">
  <img width="400" alt="image" src="https://github.com/Profzubbyd/recommender-system/assets/46527701/a9c7a548-f6c0-4716-ab62-9bf86fa9e36d">
</p>

<p align="center">
  Figure 4: Extra Trees Classifier Confusion Matrix
</p>

## VI. Conclusion
The results demonstrate that missing value imputation using classification and regression trees (cart) and predictive mean matching (pmm) yields slightly better results than random forest imputation. Extra Trees Classifier, in particular, achieves a notable accuracy of 77%. The study suggests the effectiveness of the proposed models for the in-vehicle coupon dataset. Future plans include hyperparameter tuning and exploring additional missing value imputation methods.

## References
[1] S. Barat and L. Ye, “Effects of Coupons on Consumer Purchase Behavior: A Meta-Analysis.” Journal of Marketing Development and Competitiveness, vol. 6, no. 5, pp. 131-145, 2012.

[2] Pratik K. Biswas, Songlin Liu, "A hybrid recommender system for recommending smartphones to prospective customers, Expert Systems with Applications, Volume 208, 2022, 118058, ISSN 0957-4174, https://doi.org/10.1016/j.eswa.2022.118058.

[3] Bogdan Walek, Petr Fajmon, A hybrid recommender system for an online store using a fuzzy expert system, Expert Systems with Applications, Volume 212, 2023, 118565, ISSN 0957-4174, https://doi.org/10.1016/j.eswa.2022.118565.

[4] Antonio Jesús Fernández-García, Roberto Rodriguez-Echeverria, Juan Carlos Preciado, Jorge Perianez, Juan D. Gutiérrez, A hybrid multidimensional Recommender System for radio programs, Expert Systems with Applications, Volume 198, 2022, 116706, ISSN 0957-4174, https://doi.org/10.1016/j.eswa.2022.116706.

[5] Wang, T., Rudin, C., Velez-Doshi, F., Liu, Y., Klampfl, E., & MacNeille, P. (2016). Bayesian rule sets for interpretable classification. 2016 IEEE 16th International Conference on Data Mining (ICDM). doi:10.1109/icdm.2016.0171

[6] Xiaoqian Sun, Sebastian Wandelt, Transportation mode choice behavior with recommender systems: A case study on Beijing, Transportation Research Interdisciplinary Perspectives, Volume 11, 2021, 100408, ISSN 2590-1982, https://doi.org/10.1016/j.trip.2021.100408.

[7] D. R. Hermawan, M. Fahrio Ghanial Fatihah, L. Kurniawati and A. Helen, “Comparative Study of J48 Decision Tree Classification Algorithm, Random Tree, and Random Forest on In-Vehicle Coupon Recommendation Data.” 2021 International Conference on Artificial Intelligence and Big Data Analytics, 2021, pp. 1-6, doi: 10.1109/ICAIBDA53487.2021.9689701.

[8] T.D. Quynh and H.T.T. Dung, “Prediction of customer behavior using machine learning: A case study.” Proceedings of the 2nd International Conference on Human-centered Artificial Intelligence, 2021.

[9] Pokhrel, P., and Lazar, A. (2022). Towards Machine Learning Interpretability for Tabular Data with Mixed Data Types. The International FLAIRS Conference Proceedings, 35. https://doi.org/10.32473/flairs.v35i.130611

[10] Binny Parida, Prashanta KumarPatra, Sthitapragyan Mohanty, Prediction of recommendations for employment utilizing machine learning procedures and geo-location based recommender framework, Sustainable Operations and Computers, Volume 3, 2022, Pages 83-92, ISSN 2666-4127, https://doi.org/10.1016/j.susoc.2021.11.001.

[11] Elham Asani, Hamed Vahdat-Nejad, Javad Sadri, Restaurant recommender system based on sentiment analysis, Machine Learning with Applications, Volume 6, 2021, 100114, ISSN 2666-8270, https://doi.org/10.1016/j.mlwa.2021.100114.
