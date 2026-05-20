# \# DataGovKG - Information Security Classification

# 

# An ontology-driven data governance framework for NSW small and medium-sized enterprises, demonstrating how SMEs can build data governance foundations through AI agents without requiring technical expertise in ontologies or coding.

# 

# \## Overview

# 

# This repository contains the implementation of the DataGovKG reference architecture applied to information security classification governance. The framework helps resource-constrained organisations (RCOs) operationalise compliance with NSW legislation (State Records Act 1998, PPIP Act 1998) through a three-tier ontology family coordinated by four AI agents.

# 

# \## Architecture

# 

# \- \*\*Three-tier ontology family:\*\* Umbrella ontology + Governance Context Ontology (GCO) + Domain sub-ontology (DSP)

# \- \*\*Four AI agents:\*\* Onboarding, Inference, Validator, Advisor

# \- \*\*Triplestore:\*\* Apache Jena Fuseki (Docker container)

# \- \*\*User interface:\*\* Streamlit multi-page dashboard

# \- \*\*Standards reused:\*\* W3C DPV, W3C PROV-O

# 

# \## Setup

# 

# \### Prerequisites

# 

# \- Python 3.11+

# \- Docker Desktop

# \- Anaconda (recommended) or virtualenv

# \- OpenAI API key

# 

# \### Installation

# 

# 1\. Clone this repository:

# ```bash

# &#x20;  git clone https://github.com/BushraAlsulayyim/datagovkg-information-security-classification.git

# &#x20;  cd datagovkg-information-security-classification

# ```

# 

# 2\. Create a Python environment:

# ```bash

# &#x20;  conda create -n datagovkg python=3.11 -y

# &#x20;  conda activate datagovkg

# ```

# 

# 3\. Install Python dependencies:

# ```bash

# &#x20;  pip install -r requirements.txt

# ```

# 

# 4\. Start Fuseki triplestore:

# ```bash

# &#x20;  docker run -d --name fuseki -p 3030:3030 -e ADMIN\_PASSWORD=admin stain/jena-fuseki

# ```

# 

# 5\. Load the ontology and persona data:

# ```bash

# &#x20;  python scripts/load\_fuseki.py

# ```

# &#x20;  \*Note: This script will be added in upcoming commits.\*

# 

# 6\. Open Fuseki UI: http://localhost:3030

# 

# \## Reproducibility

# 

# The `fuseki-data/` folder is excluded from version control as it is regenerated automatically from the ontology source files via the loading script. To reproduce the exact same triplestore state, simply run the installation steps above.

# 

# \## License

# 

# MIT License - see \[LICENSE](LICENSE) file for details.

# 

# \## Citation

# 

# If you use this work, please cite:

# 

# > Al Sulayyim, B., \& Bandara, M. (2025). DataGovKG: An ontology-driven reference architecture for data governance in resource-constrained organisations. \*PhD Thesis, University of Technology Sydney.\*

# 

# \## Contact

# 

# Bushra Al Sulayyim, University of Technology Sydney, bushra.alsulayyim@uts.edu.au
