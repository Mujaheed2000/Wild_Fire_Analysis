# Analysis of Brightness Levels in Canadian Wildfires: A Day and Night Comparative Study

## Course: DATA VISUALIZATION

## Authors:
- **Mujaheed Abdulmalik** (ID: 0758045) - EDA & Report
- **Nasim Dadgar** (ID: 0776543) - EDA & Storyboard
- **Sharon Mbaegbu** (ID: 0779411) - EDA & Report
- **Tife Olatunji** (ID: 0794016) - EDA & Storyboard

## Abstract
This investigation explores the changes in wildfire brightness across Canadian landscapes, focusing on differences between day and night conditions. Using exploratory data analysis (EDA) and advanced visualization tools in R, the project seeks to identify temporal and seasonal trends in wildfire intensity. The methodology combines the Nightfire algorithm, known for its effectiveness in detecting nocturnal thermal events, with a novel temperature threshold technique to detect fire events accurately. This study aims to enhance wildfire detection methods and emergency response frameworks, ultimately aiming to protect Canada's extensive forested areas.

## Introduction
Wildfires in Canada present significant challenges to both natural and human environments. Effective monitoring and management of these fires are crucial for mitigation. Recent advancements in satellite imagery have improved our understanding of wildfire dynamics, especially in terms of fire intensity and spread. However, a consistent analysis of the variability in fire brightness between day and night remains a gap in current methodologies. This study aims to bridge this gap by enhancing predictive capabilities for wildfire management and comprehending the variations in brightness levels associated with the diurnal cycle.

## Previous Work
1. **Dynamic Brightness Temperature Threshold (DBTDW) Algorithm**:
   - Developed by Ding et al., this algorithm uses remote sensing, meteorology, altitude, and NDVI data. It uniquely applies the Planck and Otsu algorithms to determine minimum brightness temperature thresholds, suitable for both day and night fire detection.

2. **VIIRS Nightfire Algorithm**:
   - Created by Elvidge et al., this algorithm employs multispectral data from the Suomi NPP VIIRS for night fire detection. It uses various spectral bands and Planck curve fitting to accurately detect and characterize high radiant emissions.

3. **Evaluation of a New Satellite-Based Method for Forest Fire Detection**:
   - This method employs historical AVHRR data to automatically generate local threshold values for fire detection. Its robust fire-discrimination capability was validated using data from the Italian Forestry Service.

4. **Improving Nocturnal Fire Detection with the VIIRS Day-Night Band**:
   - FILDA enhances night fire detection by incorporating visible-light and infrared signatures in VIIRS's day-night band. This method significantly improves the detection of smaller or cooler subpixel hotspots.

5. **Forest Fire Detection of FY-3D Using Genetic Algorithm and Brightness Temperature Change**:
   - Utilizes the FY-3D satellite's MERSI-II sensor, applying a genetic algorithm to optimize the threshold for potential fire points. It effectively reduces misjudgements in conventional hotspot detection.

## Methodology
The study processed a dataset of approximately 59,000 Canadian wildfire records, including brightness readings from various times of the day. R software and its associated packages—such as dplyr for data wrangling, ggplot2 and lubridate for visualization, and hms for time data manipulation—were used for preprocessing and analysis. Preprocessing included data cleaning due to the size of the dataset. The EDA encompassed both univariate and multivariate visual assessments.

## Results
The results of this study identify clear patterns in wildfire brightness that change from day to night, illuminating potential variances by date and informing detection strategies. The findings are highlighted using numerous exploratory data analysis techniques:

1. **Histogram**:
   - Shows the distribution of brightness values with a clear distinction between day (D) and night (N). During the day, most brightness values cluster at high levels, while at night, they spread out at lower levels.

2. **Box Plot**:
   - Summarizes the range and median of brightness. Daytime brightness has a higher median and less variability, while nighttime shows a lower median with more spread and outliers.

3. **Density Plot**:
   - Provides a smoothed curve of the brightness distribution. The day curve peaks sharply at high brightness levels, and the night curve has a broader base, indicating a more varied range of lower brightness values.

4. **Scatter Plot**:
   - Displays individual brightness measurements over time. Daytime shows consistent high brightness, while nighttime measurements are more spread out, with some higher outliers.

5. **Time Series**:
   - Tracks changes in brightness over several dates. The day line remains consistently high, and the night line stays low, with some fluctuation over time.

6. **Violin Plot**:
   - Combines the box plot and density into a shape that shows the distribution's density. The day plot is narrow and peaks high, while the night plot is wider at the bottom, indicating a broader distribution of low brightness values.

## Discussion & Conclusion
This study provided a comprehensive examination of wildfire brightness variations in Canadian landscapes, emphasizing the differences between day and night conditions. Utilizing exploratory data analysis (EDA) and sophisticated visualization tools in R, we revealed significant patterns in wildfire intensity over time. The analysis confirmed higher and more consistent brightness levels during the day, with lower and more variable levels at night, showing notable temporal fluctuations.

However, the study faced limitations, particularly in the resolution of satellite data, which may affect the accuracy of detecting smaller or cooler fires. Additionally, atmospheric conditions like cloud cover and smoke could have impacted the reliability of brightness measurements.

For future research, it is recommended to incorporate higher resolution data and advanced algorithms that can mitigate the impact of atmospheric interference. Exploring the integration of ground-based observations and leveraging machine learning techniques could further enhance the accuracy and predictive capabilities of wildfire management strategies. These improvements will not only refine our understanding of wildfire dynamics but also contribute significantly to the development of more effective wildfire detection and management systems.

## References
1. Ding, Y., Wang, M., Fu, Y., Zhang, L., & Wang, X. (2023). A Wildfire Detection Algorithm Based on the Dynamic Brightness Temperature Threshold. Forests, 14(3), 477-. [https://doi.org/10.3390/f14030477](https://doi.org/10.3390/f14030477)
2. Elvidge, C. D., Zhizhin, M., Hsu, F.-C., & Baugh, K. E. (2013). VIIRS nightfire: Satellite pyrometry at night. Remote Sensing (Basel, Switzerland), 5(9), 4423–4449. [https://doi.org/10.3390/rs5094423](https://doi.org/10.3390/rs5094423)
3. Cuomo, V., Lasaponara, R., & Tramutoli, V. (2001). Evaluation of a new satellite-based method for forest fire detection. International Journal of Remote Sensing, 22(9), 1799–1826. [https://doi.org/10.1080/01431160120827](https://doi.org/10.1080/01431160120827)
4. Data from University of Nebraska Advance Knowledge in Algorithms (Improving Nocturnal Fire Detection With the VIIRS Day-Night Band). (2016). In Journal of Technology & Science (pp. 221-). NewsRX LLC.
5. Dong, Z., Yu, J., An, S., Zhang, J., Li, J., & Xu, D. (2022). Forest Fire Detection of FY-3D Using Genetic Algorithm and Brightness Temperature Change. Forests, 13(6), 963-. [https://doi.org/10.3390/f13060963](https://doi.org/10.3390/f13060963)
