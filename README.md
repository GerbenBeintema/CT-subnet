## Code for paper "Continuous-time identification of dynamic state-space models by deep subspace encoding"

See `environment.yml` to which packages are required. (see [Managing envirments with conda](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html))

The only package this is not installed automatically when using `environment.yml` is [deepSI](https://github.com/GerbenBeintema/deepSI) (version 3.13). This package should be installed manually using the instruction on that github page.

The important notebooks are;

* `encoder-CT-train.ipynb` used to train the CT subnet
* `encoder-CT-analysis.ipynb` used to analyze the results obtained from `encoder-CT-train.ipynb`
* `latent-neural-ode-train.ipynb` used to train the ODE with exogenous inputs.
* `latent-neural-ode-analysis.ipynb` used to analyze the results obtained from `latent-neural-ode-train.ipynb`
* `EMPS-train-and-analysis.ipynb` used for training and analysis for both neural ODE and CT subnet on the EMPS benchmark 

The considered benchmarks are described and downloaded from: https://www.nonlinearbenchmark.org/

To run the the analysis you need either the estimate model or re-train using the train notebooks. The estimated model can be downloaded from: [drive](https://drive.google.com/file/d/15VSky-DtZNHJQjRfxCPOjBDs-xTCBBb3/view?usp=sharing) (426 MB)
