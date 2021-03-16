# Bucharest-Housing
University project for Deep Learning course

## Dataset description
In the dataset linked below there are over three thousand apartments listed for sale on the locally popular website imobiliare.ro. Each entry provides details about different aspects of the house or apartment:
* `Nr Camere` indicates the number of rooms;
* `Suprafata` specifies the total area of the dwelling;
* `Etaj` specifies the floor that the home is located at;
* `Total Etaje` is the total number of floors of the block of flats;
* `Sector` represents the administrative district of Bucharest in which the apartment is located;
* `Pret` represents the listing price of each dwelling;
* `Scor` represents a rating between 1 and 5 of location of the apartment. It was computed in the following manner by the dataset creator:
  * The initial dataset included the address of each flat;
  * An extra dataset was used, which included the average sales price of dwellings in different areas of town;
  * Using all of these monthly averages, a clusterization algorithm grouped them into 5 classes, which were then labelled 1-5;
  * You can think of these scores as an indication of the value of the surrounding area, with 1 being expensive, and 5 being inexpensive.<br />

Dataset Source: [Kaggle Denisa Dutca](https://www.kaggle.com/denisadutca/bucharest-house-price-dataset/kernels)

## To do
1. Get the data in a PyTorch-friendly format; think of ways of preprocessing the data (e.g. One Hot Encoding, etc.); (Don't forget to split the dataset in training and validation.)
2. Predict the `Nr Camere` of each dwelling, treating it as a _classification problem._ Choose an appropriate loss function;
3. Predict the `Nr Camere` of each dwelling, treating it as a _regression problem._ Choose an appropriate loss function;
4. Compare the results of the two approaches, displaying the Confusion Matrix for the two, as well as any comparing any other metrics that are interesting (e.g. MSE). Comment on the results;
5. Choose to predict a feature more suitable to be treated as a regression problem and then successfully solve it;
6. What values should the loss have when the predictions are random (when the network is not trained at all)?
