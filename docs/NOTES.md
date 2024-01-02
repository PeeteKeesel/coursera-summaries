
### Log 

I ran 

```bash
# ------------------------------- #
# Steps I performed a single time #
# ------------------------------- #

# Initially set up the environment.
conda create -n coursera_summaries python=3.12.0
conda activate coursera_summaries
conda install numpy pandas matplotlib seaborn scikit-learn scipy ipykernel ipython jupyter jupyterlab

# Save the environment in a file.
conda list -e > requirements.txt

# ------------------------ #
# Steps to perform onwards #
# ------------------------ #

# Create the environment.
conda create -n coursera_summaries -f requirements.txt
```

```
conda env export --from-history --name coursera_summaries > env.yml
```