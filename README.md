# Instructions

## Step 1
Check out this github repository

## Step 2
Ensure you have python3 and miniconda installed locally. 

## Step 3
CD into the git repo from your terminal. Install the following python packages if they aren't already on your machine:
`pip install -q langchain openai chromadb`.

## Step 4
Run `jupyter notebook` to launch a local instance of jupyter.
From the local instance opened in the browser, open `langchain_agent.ipynb` file

## Step 5 : Instructions to run prompts with pokemon data contained in the repo
The notebook already contains file paths, names and description pointing to the 4 pokemon files(2 text files and 2 CSV files) in the repo. The only change that's required is to add your open API key in the 2nd cell. If you don't have a key, you can get one from https://platform.openai.com/account/api-keys. After adding your key, click on `Kernel -> Restart and Run All`. (You may need to install some other python packages using pip that may be missing from your local machine)

In the last 2 cell outputS you will see the resultS for the given prompt related to pokemon stats and games associated with it. The output shows the cycle complete of the AgentExecutor chain being resolved to answer the final question.

You can edit the prompt to ask any other question related to pokemon stats, games or other information contained in the 4 pokemon files.

## Step 5 : Instructions to run prompts with your own data
In your local instance of the git repo, under the data folder,add the 2 text files and the 2 csv files that will be used to create the langchain agent.
In the `custom_langchain_agent.ipynb`, update the 4th cell to point to the correct file paths. Also add relevant file names for the added files.
Add your open api key in the 2nd cell.

Click on `Cell->Run All`.
Modify the prompt in the last cell to a question related to the input files and run the cell.







