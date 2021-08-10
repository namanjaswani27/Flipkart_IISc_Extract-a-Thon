# Winner! of Flipkart_IISc_Hackathon

## Attribute Extraction from text

# Objective
Given product description, the model should tag any attribute values by their corresponding tags.

eg : <br />
Product Description : `This Nike T-shirt is available in blue.`<br />
Desired Output  &nbsp; &nbsp; &nbsp; &nbsp; : `"O" "B_BRAND" "O" "O" "O" "O" "B_COLOR"` <br />

# Brief Approach
- Given Attribute-value pairs for all 5 categories [Accessories, Bottom Wear, Foot Wear, Top Wear, Full Wear], the input product descriptions were labeled
- This preprocessed input was fed to a BiDirectional LSTM model to train it for Named Entity Recognition task.


*Kindly refer to report.pdf for a detailed approach*

