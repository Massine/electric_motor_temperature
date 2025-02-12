# Electric_motor_temperature

Implementation of machine learning models to predict the temperature of an electric motor based on some other physical values.

The detailed explanations could be found in the report: https://github.com/Massine/Electric_motor_temperature/blob/master/04_Reports/project_report.pdf

## Important instructions
**The code was run on google colab with google drive mounted. Before running the code, some adjustments should be done**
- If it is run locally
    - The cell bellow should be deleted before running the notebook
    ```python
    from google.colab import drive
    drive.mount('/content/gdrive')
    ```
   
    - The paths should be updated according the fold structure. Example: the link bellow
    ```python
    df_raw=pd.read_csv('/content/gdrive/My Drive/Data Science/Electric_motor_temperature/01_Data/01_Raw/pmsm_temperature_data.csv') 
    ```

-	If it is run on collab with google drive as a storing drive
    - The paths should be updated according to your folder structure.

## Data
The data comes from: https://www.kaggle.com/wkirgsn/electric-motor-temperature

**License and use**:
The data owner allowed the use of the data under condition of refering to two published papers. The parpers were mentionned in the report file and can be found on there two following places https://www.researchgate.net/publication/331982128_Deep_Residual_Convolutional_and_Recurrent_Neural_Networks_for_Temperature_Estimation_in_Permanent_Magnet_Synchronous_Motors and https://www.researchgate.net/publication/331976678_Empirical_Evaluation_of_Exponentially_Weighted_Moving_Averages_for_Simple_Linear_Thermal_Modeling_of_Permanent_Magnet_Synchronous_Machines

## Folder structure
-	01_Data
    - 01_Raw : contains the file downloaded from Kaggle (https://www.kaggle.com/wkirgsn/electric-motor-temperature)
    - 02_Clean : contains the splited data into train and test
-	02_Notebooks : contains 5 notebooks. One for each step described in the report
-	03_Ressources
    - 01_Sources : contains the some papers used and cited
    - Other files : contains files generated during the study (ex: scores for each NN configuration)
-	04_Reports: contains the detailed report with all the explanations
-	README
