# Airbnb NYC - Kaggle Classification project
The intention of this mini project is to explore the data, engineer new features, do the preprocessing, perform feature selection, build the optimized model and score it on the test data under 8 hours. I will record my lessons learned and what I could have done better for future projects at the end of the notebook.

I will be implementing supervised machine learning on the Default of Credit Card Clients [dataset](https://www.kaggle.com/uciml/default-of-credit-card-clients-dataset) from Kaggle using ensemble models alongwith feature engineering and model selection. For this I will be using cleaned data acquired from Kaggle while walking through my analysis in an `.ipynb` file. Details about the dataset is provided in the notebook and below I will mention the machine learning techniques I will be using in this project.


## Default of Credit Card Clients [dataset](https://www.kaggle.com/uciml/default-of-credit-card-clients-dataset)
### Processes
`Exploratory Data Analysis`, `Preprocessing`, `Feature Engineering`, `Feature Selection`, `Hyperparameter Optimization`, `Interpretation and feature importance`, `Ensembles`

### Tools and Model
`ScikitLearn`, `pandas`, `Altair`, `SHAP`, `eli5`, `VotingClassifier`, `StackingClassifier`, `CatBoostClassifier`, `LGBMClassifier`, `Random Forest`, `MultinomialNB`, `Lasso`, `Suppor Vector Machine (SVC)`, `CountVectorizer`, `RandomizedSearchCV`, `RFECV`, `cross_validate`, `pipeline`, `column_transformer`, `SelectFromModel`, `OneHotEncoder`, `StandardScaler`, `classification_report`, `recall_score`, `f1_score`, `precision_score`, `roc_auc_score`

<br>

# To use this repo
Clone this Github repository, install the dependencies, and run the 
following commands at the command line/terminal from the root directory of the project:

```
conda env create --file env.yaml
conda activate Kaggle_projects
```
## Setting up Kaggle API
To use the Kaggle API, sign up for a Kaggle account at https://www.kaggle.com. Then go to the 'Account' tab of your user profile (https://www.kaggle.com/<username>/account) and select 'Create API Token'. This will trigger the download of kaggle.json, a file containing your API credentials. Place this file in the location `~/.kaggle/kaggle.json`. I have already included the `kaggle` package in the repo environment, and running the below script should download the required files. 

## To download the data file
Run the following commands at the command line/terminal from the root directory of the project to download the data files in a `/downloads` folder:
```
python src/download_data.py --dataset=uciml/default-of-credit-card-clients-dataset --file_path=downloads/
```

You can now run the notebook file.


# To contribute to the repository:
1. Fork the repository.
2. Add the implementation of the algorithm with a clearly defined filename for the script or the notebook.
3. Test the implementation thoroughly and make sure that it works with some dataset.
4. Add a link with a short description about the file in the [README.md](https://github.com/artanzand/Kaggle_projects/blob/main/README.md).
5. Create a pull request for review with a short description of your changes.
6. Do not forget to add attribution for references and sources used in the implementation.
