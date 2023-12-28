# Text_summarization-using-Hugging-face

Overview
This project utilizes the Hugging Face Transformers library to create a summarization pipeline using the Facebook BART-large-CNN model. The pipeline is designed to summarize text, and in this case, it focuses on providing concise summaries of narratives related to Operation Babylift.

Project Description
Operation Babylift was a historic event during the closing days of the Vietnam War, involving the evacuation of orphaned children from Vietnam to various countries. This project uses the summarization pipeline to distill detailed narratives related to Operation Babylift into succinct summaries.

Usage
To use this project, follow these steps:

Install the necessary dependencies:

bash
Copy code
pip install transformers
Copy and paste the provided code into your Python environment.

Adjust the text variable with the narrative or text you want to summarize.

Run the script to generate a summary using the BART-large-CNN model.

Example
The provided example script summarizes a narrative related to Operation Babylift. You can modify the text variable with your own content for summarization.

python
Copy code
# Use a pipeline as a high-level helper
from transformers import pipeline

# Create a summarization pipeline using the BART-large-CNN model
pipe = pipeline("summarization", model="facebook/bart-large-cnn")

# Input text for summarization
text = """
# (Your input text here)
"""

# Get the summary
result = pipe(text)

# Print the summary
print(result[0]['summary_text'])
Notes
Ensure you have an active internet connection, as the BART-large-CNN model is loaded from the Hugging Face model hub.
Credits
This project is based on the Hugging Face Transformers library. For more information, refer to the Hugging Face Transformers documentation.

License
This project is open-source and distributed under the MIT License.

Feel free to contribute, report issues, or suggest improvements!
