# Risky Business by: **Victor Molina**

---

## Resampling

Put the data into train test split, pre-processed using the standard scaler class, then proceeded to evaluate the models.

- [x] Random Oversampler
- [x] SMOTE
- [x] Cluster Centroids
- [x] SMOTEENN

*Which model had the best balanced accuracy score?*
### Random Oversampler
: 0.6274742054139422
### SMOTE
: 0.6604008283275117
### Cluster Centroids
: 0.529193911631636
### SMOTEENN
: 0.6478127480248659

The **SMOTE** model had the best balanced accuracy score

*Which model had the best recall score?*

We probably care for the best recall score in the low-risk area, as we would care to not aprove high-risk clients

### Random Oversampler
: 0.65
### SMOTE
: 0.68
### Cluster Centroids
: 0.41
### SMOTEENN
: 0.61

Again, the **SMOTE** model is the best choice with the highest recall score

*Which model had the best geometric mean score?*

### Random Oversampler
: 0.6158163429313908
### SMOTE
: 0.6601890687147326
### Cluster Centroids
: 0.5116889916409534
### SMOTEENN
: 0.6495836135666537

**SMOTE** wins again

## Ensemble

*Which model had the best balanced accuracy score?*

### Balanced Random Forest Classifier
: 0.7319327104761675
### Easy Ensemble Classifier
: 0.7324453791330763

The **Easy Ensemble Classifier** has the best balanced accuracy score by a small amount

*Which model had the best recall score?*

Using the recall score from the low-risk as it makes sense to pay attention to that particular recall score

### Balanced Random Forest Classifier
: 0.87
### Easy Ensemble Classifier
: 0.80

The **balanced random forest classifier** performs better

*Which model had the best geometric mean score?*

### Balanced Random Forest Classifier
: 0.7191062506221672
### Easy Ensemble Classifier
: 0.7423364532071993

The **easy ensemble classifier** has a higher geometric mean

*What are the top three features?*

1. total_rec_prncp
2. total_rec_int
3. last_pymnt_amnt