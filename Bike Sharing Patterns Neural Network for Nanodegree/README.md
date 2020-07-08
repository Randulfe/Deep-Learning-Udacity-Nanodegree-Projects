# Bike Sharing Pattern

In this project I have implemented a neural network to predict daily bike rental ridership. I analyse the data provided, figure out the advanatages and disadvantages of this particular dataset and build a feed forward neural network for it. 

Then I train the network with this data and test it with a subset of the data. Finally I have analysed how well does my model make predictions and tune my hyper-parameters to then test the model again until I have a satisfactory loss and accuracy.

More details regarding this specific case scenario along with the data and model analysis can be found in [the Jupyter notebook of this project](https://github.com/Randulfe/Deep-Learning-Udacity-Nanodegree-Projects/blob/master/Bike%20Sharing%20Patterns%20Neural%20Network%20for%20Nanodegree/Your_first_neural_network.ipynb).

## Results and hyper-parameter selection

This plot shows the main results obtained from my model which has used these hyper-paramters: 
- iterations = 2500
- learning_rate = 1.3
- hidden_nodes = 15
- output_nodes = 1


![plot of predictions vs actual values](https://github.com/Randulfe/Deep-Learning-Udacity-Nanodegree-Projects/blob/master/Bike%20Sharing%20Patterns%20Neural%20Network%20for%20Nanodegree/Sin%20t%C3%ADtulo.png)

## Instructions

Most relevant information is in either in `Your_first_neural_network.ipynb` or `my_answers.py`. However, if you want to use test the project and use it in your local machine, you can follow these instructions: 

1. Download the project materials from our GitHub repository. You can get download the repository with `git clone https://github.com/Randulfe/Deep-Learning-Udacity-Nanodegree-Projects/tree/master/Bike%20Sharing%20Patterns%20Neural%20Network%20for%20Nanodegree`.  
2. `cd` into the project directory.
3. Download anaconda or miniconda based on the instructions in the Anaconda lesson. 
4. Create a new conda environment: `conda create --name deep-learning python=3`
5. Enter your new environment:
        `Mac/Linux: >> source activate deep-learning`
        `Windows: >> activate deep-learning`
6. Ensure you have numpy, matplotlib, pandas, and jupyter notebook installed by doing the following:`conda install numpy matplotlib pandas jupyter notebook`
7. Run the following to open up the notebook server: `jupyter notebook`
8. In your browser, open `Predicting_bike_sharing_data.ipynb`.
9. Enjoy re-running or modifying the notebook ! 😄

If you need help running the notebook file let me know.

## License

MIT License

Copyright (c) 2020 Mateo Randulfe
