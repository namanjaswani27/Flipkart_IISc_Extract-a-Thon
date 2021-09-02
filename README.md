# Winner!!  of Flipkart IISc Hackathon 2021

# Objective : Attribute Extraction from text
Given product description, the model should tag any attribute values by their corresponding tags.

eg : <br />
Product Description : `This Nike T-shirt is available in blue.`<br />
Desired Output  &nbsp; &nbsp; &nbsp; &nbsp; : `"O" "B_BRAND" "O" "O" "O" "O" "B_COLOR"` <br />

# Brief Approach
- Given Attribute-value pairs for all 5 categories [Accessories, Bottom Wear, Foot Wear, Top Wear, Full Wear], the input product descriptions were labeled using `Distant Supervision`
- This preprocessed input was fed to a BiDirectional LSTM model to train it for Named Entity Recognition task.


*Kindly refer to **report.pdf** for a detailed approach*


# Scores on Held out validation set:

| Avg |Precision | Recall | F1-Score  |
| --------|----- |:-------------:| -----:|
| micro avg     | 0.50 |  0.38 |   0.43 | 
| macro avg     | 0.23 |  0.18 | 0.18   |
| weighted avg   |0.62 |  0.38 | 0.44  |

