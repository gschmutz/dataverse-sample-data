# Dataverse Sample Data

Populate your Dataverse installation with sample data.

## Requirements

- Python 3.4 or higher

## Installation

Clone this repo.

    git clone https://github.com/IQSS/dataverse-sample-data.git

Create a virtual environment for this project.

    mkdir ~/envs
    python3 -m venv ~/envs/dataverse-sample-data

Activate the virtual environment you just created.

    source ~/envs/dataverse-sample-data/bin/activate

Change directories into the repo that you cloned.

    cd dataverse-sample-data

Install dependencies into the virtual environment, especially [pyDataverse][].

    pip install -r requirements.txt

Copy `dvconfig.py.sample` to `dvconfig.py` and add your API token. Note that the config file specifies which sample data will be created.

## Adding sample data

Assuming you have already run the `source` and `cd` commands above, you should be able to run the following command to create sample data.

    python create_sample_data.py

[pyDataverse]: https://pypi.org/project/pyDataverse/