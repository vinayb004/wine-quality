# Wine Quality Analysis | Programming Assignment 2

## Full Readme 
* [Readme DOC](https://github.com/vinayb004/wine-quality/blob/main/report.docx)

## Docker image link
* [image](https://hub.docker.com/repository/docker/vinaybasavaraja/winequal)

## Goal:
* The purpose is to develop parallel machine learning (ML) applications in Amazon AWS cloud platform.Specifically, you will learn: (1) how to use Apache Sparkto train an ML model in parallel on multiple EC2 instances; (2) how to use Spark’s MLlib to develop and use an  ML model in the cloud; (3) How to use Dockerto create a container for your ML model to simplify model deployment.

## Description:
* To build a wine quality prediction ML modelin Spark over AWS.The model must be trained in parallel on multiple EC2 instances.Then, you need to save and load the model in an application that will perform wine quality prediction; this application will run on one EC2 instance.

## Pre-requisites :
* Input file must be copied under data/ and with same name TestDataset.csv
* Input file must have save format as of TrainingDataset.csv and ValidationDataset.csv. Column names in double quotes with exact name number of column with same names and separator ';'

## Docker run instructions
````
docker pull vinaybasavaraja/winequal:v1
````
````
docker run -v [fullLocalPath of TestDataset.csv: data/TestDataset.csv ] vinaybasavaraja/winequal:v1
```` 
for e.g.
````
sudo docker run -v /home/ec2-user/data/ValidationDataset.csv vinaybasavaraja/winequal:v1
```` 

