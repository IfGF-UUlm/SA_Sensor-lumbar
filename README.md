# SURGE-Ahead Lumbar IMU Sensor Analysis 
This GitHub repository contains the code for analyzing lumbar inertial measurement unit (IMU) sensor data within the Supporting SURgery with GEriatric Co-Management and AI (SURGE-Ahead) project.

## Project Overview
The project leverages wearable sensor technology and deep learning to objectively monitor and predict functional recovery after surgery in older adults.
A secondary analysis of data from 39 patients (mean age 79.05 years) undergoing surgery was performed, utilizing IMU sensors worn at the lumbar region for up to five postoperative days.
Deep learning models ([TabPFN](https://github.com/PriorLabs/TabPFN)) were applied to predict Charité Mobility Index (CHARMI) and Barthel Index scores, as well as discharge destination, achieving R² values of 0.65 and 0.70 for CHARMI and Barthel Index prediction, respectively, and 82% accuracy for discharge destination prediction.
These results demonstrate the promising potential of IMU-based data and deep learning for automated functional assessment and discharge decision support in this vulnerable population.

## Repository Structure
- [`Analysis.ipynb`](./Analysis.ipynb): IMU feature extraction
- [`Diaries.ipynb`](./Diaries.ipynb): Movement diary analysis
- [`IMU+DL_regression.png`](./IMU+DL_regression.png): Figure 2: Deep learning prediction of assessment scores compared to actual scores
- [`LICENSE`](./LICENSE): License for this project (MIT License, as per the project's uniform approach)
- [`Prediction-TabPFN_lumbar.ipynb`](./Prediction-TabPFN_lumbar.ipynb): Deep learning prediction from IMU data using [TabPFN](https://github.com/PriorLabs/TabPFN)
- [`SAh_OKIE_DB_20250303.xlsx`](./SAh_OKIE_DB_20250303.xlsx): Data from the (observation and AI development study)[https://github.com/IfGF-UUlm/SA_OKIE] of the SURGE-Ahead project
- [`catalog.csv`](./catalog.csv): Catalog of patient and movement diary data
- [`diary_regression.png`](./diary_regression.png): Figure 1: Gait detection performance compared to activity level
- [`results.csv`](./results.csv): Extracted IMU features as tabular data
- [`results_IMU.csv`](./results_IMU.csv): Results from IMU exploratory analysis for feature selection
- [`results_diary.csv`](./results_diary.csv): Results from the movement diary analysis


### Explore the Analysis:
- Open [`OKIE_main.ipynb`](./OKIE_main.ipynb) in GitHub to inspect IMU feature extraction
- Open [`Diaries.ipynb`](./Diaries.ipynb) in GitHub to inspect movement diary analysis
- Open [`Prediction-TabPFN_lumbar.ipynb`](./Prediction-TabPFN_lumbar.ipynb) in GitHub to inspect deep learning prediction from IMU data

**Note:** It is possible to download or clone the repository and create a virtual environment using conda: `conda env create -f environment.yml`
However, due to file size limitations the raw IMU data is not publicly available, meaning [`Analysis.ipynb`](./Analysis.ipynb) cannot be rerun. 

#### The analysis notebook utilizes:
- Python 3.x
- numpy
- pandas
- scikit-digital-health (skdh)
- mobgap
- scipy
- matplotlib
- scikit-learn (sklearn)
- tabpfn

## License
This project is licensed under the MIT License.

## Citation
For academic use, please cite the underlying manuscript (details forthcoming, provided once published):

[pending]

## Contact
Questions, Feedback, or Concerns? Reach out to thomas.kocar@uni-ulm.de.
