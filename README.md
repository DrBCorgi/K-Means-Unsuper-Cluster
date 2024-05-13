# K-Means-Unsuper-Cluster

Requirements
Python 3.x: Ensure Python is installed on your system.
Libraries: You need pandas, torch, transformers, sklearn, and openpyxl. Install them using pip if not already installed:
bash
Copy code
pip install pandas torch transformers scikit-learn openpyxl
Tkinter: Typically included with Python's standard library for GUI operations.
Instructions
Prepare Your Data:

Your input should be an Excel file where the text data for clustering is stored in the first column.
Ensure the Excel file does not contain any empty rows in the column with text data.

Running the Script:

Execute the script by running python KMeansUnsupervisedCategories.py from your command line or terminal.
Interact with GUI:

Select the Input File: A file dialog will pop up asking you to select your input Excel file. Navigate to the file's location, select it, and open it.

Review Cluster Analysis Output: The script will print cluster silhouette scores for different numbers of clusters to help determine the best clustering arrangement. It will automatically select the optimal number of clusters based on these scores.
Check Console for Cluster Details: Key terms for each cluster will be printed in the console, giving you an idea of the dominant themes or sentiments in each cluster.

Save the Output:

Choose Save Location: After processing, another file dialog will ask where to save the output Excel file.
File Contents: The output file will include:
The original data with an additional column labeled 'Cluster' indicating the cluster each row belongs to.
A summary sheet with cluster names and the count of items in each cluster.

Review the Results:

Open the saved Excel file to view the clustering results and summary. This will help in understanding the grouping and distribution of your data.

Notes:
The script uses a pre-trained model (distilbert-base-uncased) from Hugging Face's transformers library, which is suitable for general English text. If your data is very domain-specific, consider using or training a model more suited to your domain.
The script handles cases where some clusters might not have any data points, marking them as "No data" to avoid errors during processing.
