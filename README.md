# machine-learning

## Connecting dataset with Kaggle API
### 1. Install Kaggle API
``` bash
pip install kaggle
```
### 2. Go to Kaggle and get your API key
- Go to Kaggle and sign in
- Click on your profile picture on the top right corner and go to 'My Account'
- Scroll down to API section and click on 'Create New API Token'
- This will download a file called 'kaggle.json'
- Move this file to the location ~/.kaggle/kaggle.json
- If the folder ~/.kaggle does not exist, create it
- Change the permissions of the file
``` bash
chmod 600 ~/.kaggle/kaggle.json
```
### 3. Download dataset
- Go to the dataset you want to download
- Click on the '3 dots' on the right side and click on 'Copy API command'
- Run the command in your terminal
``` bash
kaggle datasets download -d <dataset-name>
```
- This will download the dataset in the current directory
- If you want to download the dataset in a specific directory, run the following command
``` bash
kaggle datasets download -d <dataset-name> -p <path-to-directory>
```
### 4. Unzip the dataset
- Unzip the dataset using the following command
``` bash
unzip <dataset-name>.zip
```
- If you want to unzip the dataset in a specific directory, run the following command
``` bash
unzip <dataset-name>.zip -d <path-to-directory>
```
### 5. Delete the zip file
- Delete the zip file using the following command
``` bash
rm <dataset-name>.zip
```