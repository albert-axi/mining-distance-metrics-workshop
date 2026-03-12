# Mining Distance Metrics Workshop Lab

This repository contains a workshop-ready lab for teaching distance metrics in a mining operations context.

## Workshop scenario

A mining operations team is monitoring equipment using site sensors. Each reading contains:

- temperature
- vibration
- pressure
- humidity

The team wants to compare readings to answer questions such as:

- Which machines are behaving most similarly?
- Which readings look unusual and may require inspection?
- How do different similarity measures change what we classify as "close"?

This lab uses those questions to introduce Euclidean distance, Manhattan distance, cosine similarity, pairwise distance matrices, and a simple clustering extension.

## Repository structure

```text
mining-distance-metrics-workshop/
├── notebooks/
│   ├── participant_distance_metrics_lab.ipynb
│   └── instructor_solution_distance_metrics_lab.ipynb
├── data/
│   └── sample_mining_sensors.csv
├── environment/
│   └── requirements.txt
└── README.md
```

## Who this lab is for

This activity is suited to participants who are new to notebook-based machine learning work through to intermediate users who want a clear, applied introduction.

## Learning goals

By the end of this activity, participants should be able to:

1. load tabular sensor data into a notebook
2. inspect data structure and summary statistics
3. compare observations using Euclidean distance, Manhattan distance, and cosine similarity
4. explain how metric choice changes the meaning of similarity
5. build a distance matrix and identify similar records
6. connect distance metrics to practical mining use cases such as anomaly review and clustering

## How to run the lab

### Option 1: Jupyter Notebook or JupyterLab

1. Create a Python environment.
2. Install the requirements:

   ```bash
   pip install -r environment/requirements.txt
   ```

3. Start Jupyter:

   ```bash
   jupyter notebook
   ```

4. Open the participant notebook in the `notebooks/` folder.
5. Run the cells from top to bottom using `Shift + Enter`.

### Option 2: Google Colab

1. Upload the repository contents to your own GitHub repository or Google Drive.
2. Open the participant notebook in Google Colab.
3. Make sure the `data/` folder stays beside the notebook or update the file path in the data-loading cell.
4. Run all cells from top to bottom.

## Teaching notes

- Use the participant notebook during the lab.
- Use the instructor notebook for worked answers and facilitation prompts.
- The guided tasks include checkpoint questions and solution cells.
- The dataset is synthetic and intended for training use.

## Suggested workshop flow

- 10 min: context and notebook orientation
- 15 min: load and inspect the dataset
- 20 min: compare two sensor readings with three metrics
- 20 min: distance matrix and nearest-pair activity
- 15 min: guided cosine similarity task
- 10 min: clustering extension and reflection

## Licence

Use and adapt for training purposes.
