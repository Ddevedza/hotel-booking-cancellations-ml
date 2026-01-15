# hotel-booking-cancellations-ml
Hotel Booking Cancellation Prediction

Machine learning project for predicting hotel booking cancellations using real Kaggle dataset. Includes preprocessing (ColumnTransformer), Logistic Regression, Random Forest, evaluation metrics and business interpretation.

Opis (srpski):
Projekt predviđa otkazivanje hotelskih rezervacija na osnovu realnog Kaggle dataset-a. Obuhvaćen je kompletan end-to-end ML tok uključujući pripremu podataka, feature engineering, modeliranje, evaluaciju i poslovnu interpretaciju rezultata.

Dataset:

  Korišćen je Kaggle dataset:
  Hotel Booking Demand Dataset (119,391 redova i 32 kolone)
  
  Link: https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand
  
  Ciljni label: is_canceled
  (1 = canceled, 0 = not canceled)


Problem i cilj:

  Otkazivanje rezervacija direktno utiče na prihod hotela i planiranje kapaciteta.
  Cilj projekta je predvideti da li će rezervacija biti otkazana na osnovu informacija dostupnih u trenutku rezervacije, i identifikovati najvažnije faktore.
  
  Sa poslovne strane primarni fokus je na recall metriku za klasu "canceled", jer propušteno otkazivanje može da košta hotel.

Metod:

  Korišćeni modeli:
  
  - Logistic Regression (baseline)
  
  - Random Forest Classifier (napredniji model)
  
  Preprocesiranje urađeno kroz Pipeline i ColumnTransformer:
  
  Numeričke vrednosti: imputacija + skaliranje
  
  Kategorijske vrednosti: imputacija + OneHot encoding
  
  Trening i evaluacija sa train_test_split (stratify=True)
  

Evaluacija:

  Korišćene metrike:
  
    - Accuracy
    
    - Precision
    
    - Recall
    
    - F1-score
    
    - Confusion Matrix
    
    - ROC-AUC
  
  Random Forest je postigao bolje rezultate od Logistic Regression-a, posebno na recall-u za klasu "canceled", što je ciljano zbog poslovnog konteksta.
  

Tehnologije:
  
  - Python
  
  - pandas, numpy
  
  - matplotlib, seaborn
  
  - scikit-learn
