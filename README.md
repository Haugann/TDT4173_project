## Ensemble of specialized convolutionalnetworks for performance enhancement
This repo is made for the final project in TDT4173 - Machine Learning by [Yathuwaran Raveendranathan](https://github.com/Yathuwaran/), [Jonas Thorset](https://github.com/JonasThorset) and [Håkon Haugann](https://github.com/Haugann). 

The main focus of this project are to see howensamblemethodsmay improve a CNN and also to see if simple modifications to the structure mayimprove overall accuracy, in the case of image classification. The ensemble is defined such that 5 specialized CNNs are combined into one ensemble by voting.

As the whole ensemble-based implementation is written in a IPython notebook, it is quite easy to run on e.g. Google Colab, where one also can attain GPU resources. The notebook containing the ensemble can be runned with pretrained data by initializing them as follows;

    best_weight = {0:"bird_and_cat.15-0.43.hdf5",1:"car_and_plane.15-0.31.hdf5",2:"deer_and_dog.15-0.35.hdf5",3:"frog_and_horse.15-0.30.hdf5",4:"ship_and_truck.15-0.32.hdf5"}
In the code each of the files contains the weights for the trained CNNs, and can be found under the `../weights/esemble` directory.

To run the code first the `Imports` and `CNN model creation for ensamble method` cells has to be runned. Further each model has to instantiated. If it is desired to use the pretrained weights, the `Training the individual models` cell is not necessary to run. The rest of the notebook can then be runned to get the results and additional visualization. 

The general CNN notebook can be runned in the same manner, with its respective weight-file.



