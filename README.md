# Stock Market Analysis

This repo contains some stock market analysis scripts. The goal is acquiring and analyzing some ﬁnancial data related to different strategies, and then making an investment decision based on these analysis.


## Getting Started

Install the requirement with the following steps:
1. Make sure you have [poetry](https://python-poetry.org/) installed.
2. Run the following command to install dependency.

    ```
    poetry install
    poetry run ipython kernel install --user --name=stock-analysis-env
    ```

Now you're ready to go!

## Usage
### Using Jupyter Notebook

The simplest way is to run jupyter notebook using:
```
poetry run jupyter notebook
```

You will see a link for you to open jupyter notebook in the browser.
**Remember to select `stock-analysis-env` as jupyter notebook kernel.**


### Using VS Code

If you're using VS Code, then make sure you have `Python` extension installed.
After that, just open the `ipynb` file in the editor and you'll see everything working.
**Remember to select `stock-analysis-env` as jupyter notebook kernel.**
The option can be located at top right corner.