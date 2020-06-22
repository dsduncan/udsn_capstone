# Udacity data science nano degree capstone project #

This is the Avarto Financial Solutions segmentation project. It consists of
analyzing data from general German consumers and customers of a mail-order
company to identify target customers for marketing campaigns. You can see a
full write-up in my [Medium post][1]. Due to the terms attached to the data
used in this project, it unfortunately can't be run as-is, so this is more of
an historical record.

## Setup ##

The project is run from the notebook `Arvato Project Workbook.ipynb`. It assumes
the following raw data files are located in the subfolder `data/`:

* `Udacity_AZDIAS_052018.csv` - general population demographic info
* `Udacity_CUSTOMERS_052018.csv` - demographic info for existing customers
* `Udacity_MAILOUT_052018_TRAIN.csv` - demographic info for recipients of a 
marketing campaign, as well as their response to same
* `Udacity_MAILOUT_052018_TEST.csv` - demographic info for recipients of a
marketing campaign, with responses withheld

In addition, there are a couple of external files that reflect configurations
needed to recreate the workflow. These are in the repo:

* `variable_eval.csv` - indicators for which features to include in the analysis
and how to treat them vis a vis null values and datatypes
* `col_drop.csv` - list of features removed during the modeling process to get
to the submitted result

## Process ##

The notebook can be run straight through, and contains chatty documentation of 
the approach. It creates three intermediate files (`variables_descs.csv`,
`variables_pairwise.csv`, `variables_segment.csv`) which were used for the 
manual part of the analysis, as well as `kaggle_submission.csv`, which
can be submitted directly to the Kaggle competition for the class. 

## Licensing & Acknowledgments ## 

The data in this project come from AZ Direct GmbH, supplied by Avarto Financial
Solutions as part of the Udacity Data Science program. I have effectively no 
ownership over the data after the program and will be deleting my local copies, 
so don't even ask for it.

[1]: https://medium.com/@clonedgoodness/customer-prospecting-for-mail-order-services-b345cbfdaa8d
