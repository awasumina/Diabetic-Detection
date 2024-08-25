# Diabetic Detection - Naive Bayes Classifier

This project implements a Naive Bayes classifier for the Pima Diabetes dataset using Python. The classifier is designed to predict the presence of diabetes in patients based on several medical attributes.

## Dataset

The dataset used in this project is the [Pima Diabetes dataset]. This dataset contains 768 rows of patient data with the following attributes:

- `Pregnancies`: Number of times pregnant
- `Glucose`: Plasma glucose concentration a 2 hours in an oral glucose tolerance test
- `BloodPressure`: Diastolic blood pressure (mm Hg)
- `SkinThickness`: Triceps skin fold thickness (mm)
- `Insulin`: 2-Hour serum insulin (mu U/ml)
- `BMI`: Body mass index (weight in kg/(height in m)^2)
- `DiabetesPedigreeFunction`: Diabetes pedigree function
- `Age`: Age (years)
- `Outcome`: Class variable (0 or 1) where 1 indicates presence of diabetes and 0 indicates absence

## Requirements

To run this code, you'll need the following Python packages:
- `csv`
- `random`
- `math`
- `google.colab` (for file upload functionality in Google Colab)

## How to Run

1. **Upload the Dataset:**
   Ensure that the Pima Indians Diabetes dataset CSV file is uploaded. You will be prompted to upload the file using the Google Colab file upload interface.

2. **Execute the Code:**
   Run the provided code in a Google Colab notebook or your local Python environment. The code will:
   - Load the CSV file.
   - Split the dataset into training and test sets.
   - Train a Naive Bayes classifier.
   - Test the classifier and calculate the accuracy.

3. **View Results:**
   The output will include:
   - The number of rows split into training and test sets.
   - The accuracy of the Naive Bayes classifier on the test set.

## Code Explanation

- **`loadCsv(filename)`**: Loads the CSV file and converts data to float values, skipping the header.
- **`splitDataset(dataset, splitRatio)`**: Splits the dataset into training and test sets based on the provided split ratio.
- **`separateByClass(dataset)`**: Separates data into classes for Naive Bayes calculations.
- **`mean(numbers)`**: Calculates the mean of a list of numbers.
- **`stdev(numbers)`**: Calculates the standard deviation of a list of numbers.
- **`summarize(dataset)`**: Summarizes the dataset by calculating mean and standard deviation for each attribute.
- **`summarizeByClass(dataset)`**: Summarizes the dataset by class.
- **`calculateProbability(x, mean, stdev)`**: Calculates the probability of an attribute value given its mean and standard deviation.
- **`calculateClassProbabilities(summaries, inputVector)`**: Calculates class probabilities for a given input vector.
- **`predict(summaries, inputVector)`**: Predicts the class label for a given input vector based on class probabilities.
- **`getPredictions(summaries, testSet)`**: Gets predictions for the test set.
- **`getAccuracy(testSet, predictions)`**: Calculates the accuracy of the classifier.

## Results

Upon running the code, you will see the following output:

```
Split 768 rows into train 514 and test 254 rows
Accuracy: 62.99%
```

This indicates the model has an accuracy of approximately 63% on the test dataset.

## Notes

- The accuracy may vary slightly due to the random splitting of the dataset.
- This implementation uses a simple Naive Bayes classifier and can be further optimized or compared with other classification algorithms for better performance.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to adjust the README to better fit your specific needs or preferences!