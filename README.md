# **README**

**Platform**

MacOS Sonoma 14.3.1


**Steps**

* clone repo https://github.com/MarkiesFredje/pyspark-exercise
* read instructions in notebook
* brew install openjdk@11
* created virtualenv with pyenv
* pip installed jupyter findspark pyarrow pandas keyring
* start jupyter-notebook
* point env vars to my dirs
* set spark local ip env var
* implement notebook
* uploaded notebook to Google Colab space


Initially, the code was written with Pandas DataFrames.
I'm on a tight schedule.

Setting up Spark inside Colab was done in another way.
Java is already installed there, so skipped.

Migration to use RDD DataFrames after a Pandas version was implemented.

The schema was deduced from the superset, and used while loading the data from JSON

GDPR compliance: the sensitive data was encrypted with a strong AES key. The key is stored in a Google Colab secret.

Data is written to a parquet file, with partitioning on branch ID




