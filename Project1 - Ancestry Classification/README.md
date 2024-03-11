# Advanced Ancestry Classification Through Machine Learning 

Problem: The project addresses the significant challenge of leveraging Single Nucleotide Polymorphism (SNP) data for accurate ancestry prediction. 
The high dimensionality of SNP data, where the feature space significantly surpasses the number of samples, introduces complexity in model training, leading to potential overfitting and reduced prediction accuracy. 

This repository contains a series of Jupyter notebooks dedicated to the application of machine learning techniques for the purpose of advanced ancestry classification using Single Nucleotide Polymorphism (SNP) data. The project utilizes a comprehensive dataset from the 1000 Genomes Project, aiming to improve the accuracy and understanding of genetic ancestry predictions.

## Project Structure

The repository is organized into a series of Jupyter notebooks, each serving a specific role in the data analysis and model development pipeline:

1. **VCF_to_CSV.ipynb**
   - Description: Converts VCF files into a more manageable dataframe format for further analysis.
   
2. **Preprocessing.ipynb**
   - Description: Performs cleaning and preprocessing on the genetic data, including handling missing values and applying quality control measures.
   
3. **Scatter_Plots_SuperPopulation.ipynb**
   - Description: Generates scatter plots using PCA, SVD, t-SNE, and UMAP labeled with 5 general ancestry population codes: AMR, AFR, SAS, EAS, EUR.
   
4. **Scatter_Plots_Population.ipynb**
   - Description: Creates scatter plots using PCA, SVD, t-SNE, and UMAP labeled with 26 detailed ancestry population codes.
   
5. **Model_Development_SuperPopulation.ipynb**
   - Description: Develops classification models for the 5 general ancestry populations, evaluates them using cross-validation, and reports the results with metrics such as ROC and confusion matrices.
   
6. **Model_Development_Population.ipynb**
   - Description: Similar to the previous notebook but focuses on developing models for the detailed 26 ancestry populations.
   
7. **Component_Analysis_SuperPopulation.ipynb**
   - Description: Conducts an iterative process to determine the impact of increasing the number of components on model performance for the 5 general ancestry populations.
   
8. **Component_Analysis_Population.ipynb**
   - Description: Applies an iterative process to analyze how increasing the number of components affects model performance for the 26 detailed ancestry populations.
   
9. **Performance_SuperPopulation.ipynb**
   - Description: Compares final results, plotting how AUC and F-1 scores change with the iterative process of increasing the number of components for the 5 general ancestry populations.
   
10. **Performance_Population.ipynb**
    - Description: Compares final results for the 26 detailed ancestry populations, focusing on changes in AUC and F-1 scores with the increase in the number of components.

## Installation and Usage

To run the notebooks in this repository, ensure that you have Jupyter Notebook or JupyterLab installed. If not, you can install it using pip:

```bash
pip install notebook
```

Clone the repository to your local machine:

```bash
git clone https://github.com/bmamandipoor/CSE-284---Personal-Genomics.git
```

You can then open and run the individual notebooks from the Jupyter Notebook interface in your browser.

## Dependencies

This project relies on several Python libraries such as NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn, and UMAP-learn. Ensure these are installed in your environment:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn umap-learn
```

## Acknowledgments

- 1000 Genomes Project for providing the genetic dataset.
- Contributors and maintainers of the Python packages used in this project.
