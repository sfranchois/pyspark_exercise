# **README**

**Platform**

MacOS Sonoma 14.3.1


**Steps**

In short

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
* Upload the notebooks to GitHub and share the repo

Initially, the code was written with Pandas DataFrames.
I'm on a tight schedule. Professionally, we used Pandas a lot. Spark was a long time ago. 

Setting up Spark inside Colab was done in another way.
Java is already installed there, so skipped.

Migration to use RDD DataFrames was implemented after the Pandas version was completed, which served as a skaffold.

The schema was deduced from the superset, and used while loading the data from JSON. 
As a validition, each file is checked if it contains data.

GDPR compliance: the sensitive data was encrypted with a strong AES key. The key is stored in a Google Colab secret.
Without this key, noone can read it.

Data is written to a parquet file, with partitioning on branch ID




