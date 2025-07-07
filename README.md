# Capstone_mini_project
This repository contians a price prediction model based on real time data for multiple parking slots coming in at the same time.
There are two models in this repository one is fairly simple based on a few parameters and the other one has more complexity with higher number of parameteres...

Tech stack used-> Numpy, Pandas, Matplotlib for model implementation and debugging. Pathway, Bokeh for real time data streaming and processing.
Assumption- The price of next day ticket can be estimated using previous day parameters.

1. Simple Model
   This model will only use the Codes,Occupancy and capacity of the parking lot to predict the price of parking ticket for the next day...

   The data is injected in real time using pathway and the price is calculated by using basic functions only..

   The visualisations that will be included will are created by using Bokeh in streaming mode. Visualization for one parking lot has been included.

   The objective function used here is the difference between the maximum and minimum occupancy during a day to depict the potiential scarcity of
   customers which is then normalized using a sigmoid function and then added in the base price....
   ![image](https://github.com/user-attachments/assets/254ae88e-24df-4160-aef0-41a7072723aa)
3. Complex Model

   This model will use parameters like Codes,Occupancy,Capacity, Nearby traffic conditions, Special day, queue length and a demand function for        every parking lot.The data is injected in real time using pathway and the price is calculated by using demand based function. For visualisation
   Bokeh has been used.'

   The Objective function is a linear combination of these parameters with carefully tuned coefficients and normalization using sigmoid function to    catch the underlying relationship in data and predict prices efficiently using a broader set of parameters.
  ![image](https://github.com/user-attachments/assets/4ebb6922-e966-4043-9b80-7ebe891319a9)

