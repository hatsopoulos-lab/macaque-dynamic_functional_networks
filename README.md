# DynamicStructure-2022
codebase for "Dynamic Structure Of Motor Cortical Neuron Co-Activity Carries Behaviorally Relevant Information"

On [bioArxiv](https://doi.org/10.1101/2022.05.18.492501)

## Set up environment (Linux)
On the terminal:
1. Clone Repository `gh repo clone mjms/DynamicStructure-2022`
2. Create conda environment: `conda env create -f environment.yml`
3. Activate conda environment `conda activate reach-analysis`

All the code in this repository is run on Jupyter Notebooks.

The functions used are found in `ms_packages_and_functions.ipynb`
To load the functions into a new notebook, run this at the start of your notebook:
`%run ../ms_packages_and_functions.ipynb`

or use `center-out/ipynb-template.ipynb` 

## Data Structure
Data can be made available upon request to Marina Sundiang (sundiang@uchicago.edu).

load data: `data = loadPickle(filepath)`

find data structure and example functions (including how to construct Functional Networks) under ` DynamicStructure-2022/center-out/run_data_demo.ipynb `

## Running analyses and generating figures
Each analysis has its own `run_<analysis>.ipynb` and corresponding figures have their own notebooks `All_<analysis>_plotting+statistics.ipynb`
#### Fig 2. Correlational structure of full trial FNs are specific to reach target direction.
  1. `run_UMAP_embedding_fullTrial.ipynb`
  2. `All_static-UMAP-GAS_plotting+statistics.ipynb`
#### Fig 3. Trajectories of single trial temporal FNs through a low-dimensional subspace. 
  1. `run_UMAP_embedding.ipynb`
  2. `All_temporal-UMAP-embedding_plotting+statistics.ipynb`
#### Fig 4. Graph alignment scores between FNs reflect distance of reach targets.
  1. `run_null-metrics_GAS.ipynb`
  2. `All_temporal-GAS_plotting+statistics.ipynb`
#### Fig 5. Decoders that incorporate pairwise spike time statistics predict reach direction more accurately. 
  1. `run_Decoder.ipynb`
  2. `All_temporal-decoder_plotting+statistics.ipynb`
####  Fig 6. Reciprocity decreases shortly after instruction. 
  1. `run_null-metrics_reciprocity.ipynb`
  2. `All_temporal-reciprocity_plotting+statistics copy.ipynb `

#### Additonal notebooks:
1. To generate rate-matched null FNs: `run_rate-matched-poisson-200ms-window-multiprocess.ipynb`

