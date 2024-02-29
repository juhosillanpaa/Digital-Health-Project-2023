Here is a guide on how to run the files!

Everything can be run inside the jupyterhub for the course.
However, there can be issues with the memory as the acceleration data is very large.

1. load data
Download the dataset from this source and place the data folder to the same directory
as the notebooks.
https://physionet.org/content/sleep-accel/1.0.0/
If you are unable to save all data to jupyterhub, select only few subjects and save only their data.

2. preprocessing

Run following files in order:
labels_preprocess.ipynb
heart_rates_preprocess.ipynb
accelerations_preprocess.ipynb
training_data_generator.ipynb

If you selected only certain subjects, alter the beginning of the notebooks where there is a list of
subject ids.


3.analysis
run notebook analysis.ipynb

When train test split is done, there is variable for controlling the amounf of data that is used.
To speed things up, use n = 10**4, it should still get good results in RFC.

PS. MLP and Gradient Boosting take forever.

4. Files for initial data inspection and exploration. Might contain some incorrect stuff that is
done differently in the actual preprocessing steps.

digital_health_preprocess.ipynb
digital_health_project_analysis.ipynb. - contains bad data and not good results.


