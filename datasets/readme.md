**Download**

Download the experimental data lists from [Data_lists repo](https://huggingface.co/datasets/The_data_will_be_released_upon_acceptance_of_the_paper) and extract them into the `Data_lists/` directory to obtain `Families.json`, `TRAIN.json`, `TEST.json` and `TEST_forUnknownAttack.json`.

Download the meta data from [Meta_data repo](https://huggingface.co/datasets/The_data_will_be_released_upon_acceptance_of_the_paper) and extract it into the `Meta_data/` directory.

**File descriptions:**  
   - `Data_lists/` — Directory containing all data lists needed for both the main experiments and the ablation study.
    - `Families.json` — List of families used in the experiments.
    - `TRAIN.json` — List of training data samples.  
    - `TEST.json` — List of test data samples.  
    - `TEST_forUnknownAttack.json` — List of an additional independent test set containing 9,000 normal samples and 10,000 unknown attack samples.
   - `Meta_data/` — Directory containing all the raw data required for both the main experiments and the ablation study. 
   
**Preprocessing (recommended):**
- To facilitate experiments, we recommend first running:  
     ```bash
     python get_npz_convenient.py
     ```  
- This script reads the raw data (text) in `Meta_data/` and converts each sample into a `.pkl.gz` file with the same name.  
- The generated `.pkl.gz` files are also saved in the `Meta_data/` directory.