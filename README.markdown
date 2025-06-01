# Alloys Composition Analysis

This Jupyter notebook analyzes a dataset of alloys, parsing their compositions and performing clustering analysis.

## Dependencies

- Python 3.x
- pandas
- odfpy
- numpy
- matplotlib
- scikit-learn

Install the required packages using:

```bash
pip install pandas odfpy numpy matplotlib scikit-learn
```

## Usage

1. Place the dataset file `BMGs-2024.ods` in the `data` directory.
2. Run the notebook cells in order using Jupyter Notebook or JupyterLab.

## Code Summary

1. **Data Loading**: Reads the Excel file `BMGs-2024.ods` using odfpy.
2. **Composition Parsing**: Uses regular expressions to parse the "Alloys (composition)" column, extracting elements and percentages.
3. **Data Transformation**: Creates new columns for each unique element and fills them with corresponding percentages.
4. **Clustering**: Performs K-means clustering on the scaled data.
5. **Visualization**: Uses PCA to reduce dimensions and plots the clusters.
6. **Evaluation**: Calculates the silhouette score for the clustering.

## Output

- A scatter plot showing the clusters in the PCA-reduced space, saved as `clusters.png`.
- The silhouette score indicating the quality of the clustering, printed to the console.

## Notes

- The dataset must have a "Alloys (composition)" column with correctly formatted data (e.g., `Ag30.8 Ca30.8 Mg23.1 Cu15.4`).
- The number of clusters (`k`) is set to 3 by default. Adjust as needed in the clustering step.
- Ensure all dependencies are installed to avoid execution errors.