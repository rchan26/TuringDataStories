This project uses [Poetry](https://python-poetry.org/) for dependency management.
Make sure you have Poetry installed on your machine.

## Notebooks

Notebooks are in the `notebooks` directory and currently assume that there is a `data/` folder in this directory (we haven't uploaded the data here as the files are too large). You can download the dataset from [British Library Research Repository](https://bl.iro.bl.uk/concern/datasets/308c54ce-31b1-4cb1-b257-7b288a3c7926). 

The [`data_processing`notebook](notebooks/data_processing.ipynb) contains the code for processing the data and creating the dataset used in the other notebooks. In these other notebooks, the data is loaded from the `data/` folder and saved in a csv file named `"cleaned_EThOS_CSV_202304.csv"`.

## Environment setup

From this directory and in a virutal environment, run:
```bash
poetry shell
poetry install
```

Note you can alternatively use another virtual environment manager like `conda`, `venv`, or `virtualenv`. In that case, just run `poetry install`.

For using within Jupyter, you can create a kernel with:

```bash
python -m ipykernel install --user --name ethostds
```