## Running the code

1. The main result of this paper can be reproduced via running the scripts/main_vae.py file:

    `cd scripts && python main_vae.py`

2. Download the dataset you want to run with

    `python setup_data.py --dataset=DATASET_OF_CHOICE`

Default is *ml-20m*. Other options are `amazon`, which is my original furniture review data from amazon review data.

## Main Scripts

All of the scripts used to generate data are located in the `./scripts` directory.
* `main_vae.py` is MultiVAE model with and without the critic, on all datasets.
* `main_wmf.py` is used to generate results for the Weighted Matrix Factorization model on all 3 datasets.
* `main_dae.py` is used to generate results for MutliDAE on ml-20m with and without the Critic
* `ncf_training.py` is used to generate results on the datasets we compare to Neural Collaborative Filtering.
* `gather_data.py` is used to gather statistics from a fully trained model,.
* `setup_data.py` is used to download, extract, and process the data.