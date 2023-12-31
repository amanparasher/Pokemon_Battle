# Pokemon Battle Outcome Predictor

## Overview
Just a simple project for predictiong the outcome of battle between two pokemons using different classification models by feeding them a dataset containing stats of each pokemon.The dataset includes information about Pokemon attributes and battle outcomes. Three classifiers, namely Random Forest Classifier, Decision Tree Classifier, and K-Nearest Neighbor, are employed for predictions.

## Getting Started

### Prerequisites

Make sure you have the following Python libraries installed:

- pandas
- numpy
- matplotlib
- scikit-learn

### Installation

Clone the repository to your local machine:

```bash
git clone https://github.com/amanparasher/Pokemon-Battle-Outcome-Predictor.git
```

## Usage

1. Install the required libraries mentioned in the Prerequisites section.

2. Download the dataset files (`pokemon.csv` and `combats.csv`) and place them in the project directory.

3. Run the Jupyter notebook or Python script to execute the code.

```bash
python pokemon_battle_predictor.py
```

## Data Visualization

Visualizations are included to explore the distribution of Pokemon types and generations.

- Bar chart showing the number of Pokemon for each type.
- Pie chart representing the percentage distribution of Pokemon across generations.

## Data Preprocessing

1. Checked for null values and filled missing data in the "Name" column.
2. Handled missing values in the "Type 2" column by replacing them with "NA."
3. Converted categorical data to numerical values.
4. Used FeatureHasher to convert "Type 1" and "Type 2" columns.
5. Converted the dataset into a new format: (pokemon_1_data, pokemon_2_data, winner).

## Classification Models

Three classification models were implemented:

1. **Random Forest Classifier:**
   - Achieved an accuracy of 94.88%.
   - Explored the impact of varying `n_estimators` on accuracy and training time.

2. **Decision Tree Classifier:**
   - Achieved an accuracy of 93.84%.

3. **K-Nearest Neighbor:**
   - Achieved an accuracy of 87.576%.

## Hyperparameter Tuning

Tuned the Random Forest Classifier by experimenting with different values of `n_estimators` to improve accuracy. Plotted graphs to visualize the relationship between `n_estimators`, testing accuracy, and training time.


## Conclusion

- The Random Forest Classifier with 400 `n_estimators` achieved the highest accuracy of 94.943%.
- The project demonstrates the use of machine learning classifiers to predict Pokemon battle outcomes based on their attributes.

Feel free to explore and modify the code for further improvements and analysis. Enjoy predicting Pokemon battles!






## References

* Blog for initial reference [here](https://towardsdatascience.com/become-a-pok%C3%A9mon-master-with-machine-learning-f61686542ef1)

* Datasets can be found on [kaggle](https://www.kaggle.com/datasets/terminus7/pokemon-challenge)

* The official documentation for [Scikit-learn](https://scikit-learn.org/stable) and [matplotlib](https://matplotlib.org/stable/api/index)
