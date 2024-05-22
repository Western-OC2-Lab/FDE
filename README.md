# Thwarting Cybersecurity Attacks with Explainable Concept Drift

This code provides the implementation details of a Feature Drift Explanation (FDE) module responsible for identifying drifts
in a Deep Learning (DL) regression problem. The use case relates to a cyber-security attack that targets the readings of specific
sensors supplying data for a 1-dimensional Convolutional Neural Network (1D-CNN) that predicts CO2 concentrations to aid 
Heating, Ventilation, and Air Conditioning (HVAC) systems in their activations. As such, finding the compromised sensors 
via FDE allows for a targeted mitigation strategy that potentially reduces the HVAC system's energy consumption and maintains 
the occupant's comfort. 

The code documentation aligns with the content of the manuscript, which is accepted as part of the 
_International Wireless Communications and Mobile Computing Conference_ 2024 conference. The pre-print for this manuscript 
can be found using the following link: **https://arxiv.org/abs/2403.13023**

Before running the code available in the `FDE_Notebook.ipynb`, it is imperative to retrieve the data used for this paper. This can be achieved 
using the following steps:
1. Download the data used for this work, which can be found using this link: https://zenodo.org/record/3774723#.ZGEhAHbMKUl. In this repository, the 
authors provided the `prepare.py` file to generate continuous chunks of data (60 minutes). This produces two files: 1) `continuous_sections_60_train.pickle` and 2) `continuous_sections_60_test.pickle`. 
2. Create the `data` folder in the root directory, which is on the same level as `FDE_Notebook.ipynb`. Move the two generated files, `continuous_sections_60_train.pickle` and `continuous_sections_60_test.pickle`
to this directory. 

This concludes the steps required before running the `FDE_Notebook.ipyb` notebook. This notebook includes extensive 
explanation about the steps involved in the **FDE** process. 

We also included a `models` directory. In that directory, two models, which were used to generate the paper's results, are available: 
- `cnn_model.pt`: the 1D-CNN model used for CO2 level predictions.
- `ae_full_model.pt`: the auto-encoder used for retrieving the activations' latent representation.

# Contact-Info

Please feel free to contact me for any questions or research opportunities. 
- Email: shaeribrahim@gmail.com
- Gihub: https://github.com/ibrahimshaer and https://github.com/Western-OC2-Lab
- LinkedIn: [Ibrahim Shaer](https://www.linkedin.com/in/ibrahim-shaer-714781124/)
- Google Scholar: [Ibrahim Shaer](https://scholar.google.com/citations?user=78fAJ_IAAAAJ&hl=en) and [OC2 Lab](https://scholar.google.com/citations?user=ICvnj9EAAAAJ&hl=en)
