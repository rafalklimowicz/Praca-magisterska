# Praca-magisterska
* [Wprowadzenie](#wprowadzenie)
* [Technologie](#technologie)
* [Opis](#opis)

## Wprowadzenie
Celem projektu było wykorzystanie głębokich sieci neuronowych do ekstrakcji cech obrazu materiału komórkowego. Uzyskane cechy zostały następnie wykorzystane do klasyfikacji obrazów różnych rodzajów zmian nowotworowych.
	
## Technologie
Projekt został stworzony w z wykorzystaniem:
* Python 3
* Tensorflow 2
* Scipy
* Numpy
* Pandas
* Keras
* OpenCV
	
## Opis
W repozytorium znajduje się 6 notatników:

* Generate_TFRecords_Train_Test.ipynb - odpowiada za generację plikow TFRecords z łatkami wyciętymi z oryginalnych obrazu materiału komórkowego.
* Train_Evaluate_Models_Benign.ipynb i Train_Evaluate_Models_Malignant.ipynb - odpowiadają za wytrenowanie modeli autoenkoderów w oparciu o różne rodzaje zmian nowotworych, wykorzystują w tym celu pliki TFRecords.
* Generate_Features.ipynb - odpowiada za generację cech w oparciu o część kodującą autoendkodera.
* Generate_Residuum.ipynb - odpowiada za generację cech w oparciu o błąd rekonstrukcji obrazu (residuum).
* Prediction.ipynb - odpowiada za dokonanie predykcji z wykorzystaniem klasycznych modeli klasyfikacji na podstawie uzyskanych cech obrazu.
