# Questions Answered
1. **What impact resulted from increasing or decreasing the training window?** The Support for each score was the most impacted metric beacause of the increased data size. It didn't lead to a jump in accuracy though.
2. **What impact resulted from increasing or decreasing either or both of the SMA windows?** Once again no major change in accuracy but we did see a positive correlation with the size of the SMA windows and the Support Score
3.  **Did this new model perform better or worse than the provided baseline model? Did this new model perform better or worse than your tuned trading algorithm?** It was loads better at determining the selling positions (-1.0) but had 0 precision/ recall for the positives so it's the opposit of the initial one. Recommendation would be a third model that learns off both and applies it to accurately determing both positive and negative




# Model Analysis


## Initial ML Model Settings
- 3 Month Offset
- 1 hour Offset
- SVM Settings
    - C = 1
    - random state = 1

### Results
- Precision(-1): 0.0
- Precision (1): 0.56
- Recall (-1): 0.0
- Recall (1): 1.0
- F1 (-1): 0.0
- F1 (1): 0.72
- Support (-1): 1804
- Support (1): 2288
- Accuracy: 0.56



## ML Model2 Settings
- 6 Month Offset
- 1 hour Offset
- SVM Settings
    - C = 3
    - random state = 1

### Results
- Precision(-1): 0.0
- Precision (1): 0.56
- Recall (-1): 0.0
- Recall (1): 1.0
- F1 (-1): 0.0
- F1 (1): 0.72
- Support (-1): 1732
- Support (1): 2211
- Accuracy: 0.56



## ML Model3 Settings
- 18 Month Offset
- 1 hour Offset
- SVM Settings
    - C = 500
    - random state = 1

### Results
- Precision(-1): 0.0
- Precision (1): 0.56
- Recall (-1): 0.0
- Recall (1): 1.0
- F1 (-1): 0.0
- F1 (1): 0.72
- Support (-1): 1430
- Support (1): 1843
- Accuracy: 0.56


## ML Model4 Settings
- 1 Month Offset
- 1 hour Offset
- SVM Settings
    - C = 500
    - random state = 1

### Results
- Precision(-1): 0.0
- Precision (1): 0.56
- Recall (-1): 0.0
- Recall (1): 1.0
- F1 (-1): 0.0
- F1 (1): 0.72
- Support (-1): 1828
- Support (1): 2324
- Accuracy: 0.56


## ML Model5 Settings
- 12 Month Offset
- 24 hour Offset
- SVM Settings
    - C = 15
    - random state = 100

### Results
- Precision(-1): 0.0
- Precision (1): 0.56
- Recall (-1): 0.0
- Recall (1): 1.0
- F1 (-1): 0.0
- F1 (1): 0.72
- Support (-1): 1497
- Support (1): 1931
- Accuracy: 0.56