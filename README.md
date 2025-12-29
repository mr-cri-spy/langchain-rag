Langchain RAG 
Install dependencies
Do the following before installing the dependencies found in requirements.txt file because of current challenges installing onnxruntime through pip install onnxruntime.

For MacOS users, a workaround is to first install onnxruntime dependency for chromadb using:
conda install onnxruntime -c conda-forge
See this thread for additonal help if needed.

For Windows users, follow the guide here to install the Microsoft C++ Build Tools. Be sure to follow through to the last step to set the enviroment variable path.
Now run this command to install dependenies in the requirements.txt file.

pip install -r requirements.txt
Install markdown depenendies with:
pip install "unstructured[md]"
Create database
Create the Chroma DB.

python create_database.py
Query the database
Query the Chroma DB.

python query_data.py "how many country in this world?"
