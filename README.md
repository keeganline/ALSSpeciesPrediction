# SpeciesPrediction
Repostitory for tree species prediction work using LiDAR data

## Abstract
The goal of this study was to produce models capable of classifying trees in Northern Arizona forests into tree species groups. A sample of 810 trees was collected from the Coconino National Forest near the Mogollon Rim, consisting of 8 different species, four coniferous and four deciduous. After trees were individually segmented from the airborne LiDAR data, a series of metrics was calculated that were used as predictors to classify species groups (coniferous or deciduous), subclasses (pine or fir), and individual species. Multiple different models were tested, such as random forest and penalized regression, but logistic regressions picked with stepwise selection achieved the highest accuracies. Stepwise logistic regression models had the highest balanced accuracy, with the best models averaging around 84.7% accuracy in predicting coniferous or deciduous. From that, similar logistic regressions were able to provide 74.5% accuracy in classifying fir versus pine and similar subclasses. For species-level predictions, multinomial regression achieved a balanced accuracy between 66.1% to 68.0%. From these results, we can see that logistic regressions can achieve good results for the classification of tree classes and tree species in forest systems using airborne LiDAR metrics.

## Methods
* 810 trees were sampled from the Mogollon Rim in northern Arizona consisting of 8 different species:
  *   White Fir
  *   White Pine
  *   Ponderosa Pine
  *   Douglas-Fir
  *   New Mexican Locust
  *   Aspen
  *   Gambel Oak
  *   Bigtooth Maple
* Airborne LiDAR (ALS) data was recorded for the region with each tree being segmented from the overall point cloud.
* Trees were then matched with the point cloud and over 200 metrics were calculated for each one.
* 3 different classifactions were tested:
  * Coniferous vs. Deciduous
  * Conifer Subclass Groupings (i.e. Pine vs. Fir)
  * Individual Conifer Species
* Models tested were logisitic regression (simple, complex, penalized), multinomial regression and boruta random forest.
* Each model was selected and cross validated 200 times and tested on independent test data.
* Best resulting model for each model type were selected.

## Results
tbd...

## Images
