# Fourth Year Dissertation Project

## Project overview

### Project motivation

University class sizes are rapidly increasing year on year (Clancy and Goastellec 2007) while
students are expecting the same amount of contact and support from their lecturers and other
academic support staff. This has resulted in challenges for universities to support students to their
best ability and identify which students are at a risk of falling behind early on in their course.
Currently, early warning systems that utilise predictive models have been identified as a possible
solution and could help universities utilise their resources more effectively. These systems use
student’s learning analytics data from a variety of sources to make predictions about a student’s
performance. However, very few studies have presently addressed the acceptability and ethicality
of utilising student’s learning analytics data for early warning systems and students’ opinions of
being constantly monitored while learning.

### Project aims

This dissertation aims to review the acceptability of early warning systems utilising predictive
models to classify students by running ethical evaluations on students’ who would be affected
by this type of system. We will develop multiple predictive models for several courses to predict
students’ possible risk of falling behind. The models will be utilised to find when the predic-
tions become helpful for a course and what data is required to develop effective models. The
performance of the models will be evaluated alongside the acceptability of early warning systems
using theoretical framework of acceptability. We will review the possible acceptability and
ethical considerations with current systems and evaluate our predictive models with a students’
perspective. Lastly, we aim to discuss how future research into the field could be improved to
provide more ethical and acceptable solutions to the problem

## Repository purpose

This repository holds my dataset which I have used to train and evaluate my predictive models and the Jupyter Notebooks which were used in the development and pre-processing of the predictive models and dataset.

## Repository structure

- `dataset`
  - `anonymisedOUDataSet` this folder holds the raw Open University Learning Analytics Dataset (Kuzilek et al. 2017) used by this project. OULAD dataset is anonymised dataset from the Open University containing seven csv files. [OULAD website](https://analyse.kmi.open.ac.uk/)
  - `Deadline` this folder contains proccesed dataset which has been split by set-intervals in the module and by module itself
- `notebooks`
  - `explore_dataset-initial_predictions` this folder contains the initial Jupyter Notebooks which were used to explore the OULAD dataset and make some simple naive predictive models
  - `prepare_dataset` this folder contains the pre-processing Jupyter Notebooks which are required to process our dataset before being used by to train and evaluate our predictive models. The _`oulad_split_dataset_by_module.ipynb`_ file is no longer needed to be used as _`oulad_prepare_dataset.ipynb`_ splits the dataset by module as part of the pre-processing pipeline
  - `final_models` this folder contains our final predictive model which were developed for this project. Jupyter Notebooks have been split by module; however, an additional Jupyter Notebook combines all module predictive models into a single notebook to simplify generation graphs to summarise the results

## Running notebooks

All notebooks are Jupyter Notebooks.

Development has occured using Google Colab throughout this project; however, the notebooks will also work locally too.

They require the following Python libraries to run:

- matplotlib
- seaborn
- numpy
- pandas
- scipy
- sklearn
- imblearn

### Set up using Google Colab

If you plan to run the notebooks using Google Colab, the repository will have to be manually uploaded to a Google Drive account. From their the notebooks will be accessible to open. GDrive directory paths will have to be updated to the location which the OULAD dataset is stored on your GDrive. Due to the size of the dataset.

### Running localy

If running locally, Anaconda is recommended to run these scripts as Jupyter Notebook and the required Python libraries are pre-installed as part of the installation - https://www.anaconda.com/products/distribution

## References

Clancy, P. and Goastellec, G. (2007) ‘Exploring Access and Equity in Higher Education: Policy and Performance in a Comparative Perspective’, Higher Education Quarterly, 61(2), pp. 136–154. doi:10.1111/j.1468-2273.2007.00343.x.

Kuzilek, J., Hlosta, M. and Zdrahal, Z. (2017) ‘Open University Learning Analytics dataset’, Scientific Data, 4(1), p. 170171. doi:10.1038/sdata.2017.171.
