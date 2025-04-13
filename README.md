# Sorting Algorithm Implementation & Visualization

## Overview

This Jupyter Notebook (`sorts.ipynb`) provides Python implementations of three common sorting algorithms: Bubble Sort, Insertion Sort, and Merge Sort. It includes basic tests and, more importantly, code to measure the execution time of these algorithms on randomly generated arrays of varying sizes.

The key feature is an interactive plot generated using `matplotlib` and `ipywidgets`, which visually compares the time complexity (time taken vs. array size) of the implemented sorting algorithms. Users can interactively adjust the maximum array size displayed on the plot and toggle the plot's visibility.

## Features

*   **Implementations:**
    *   Bubble Sort (O(n^2) average/worst case)
    *   Insertion Sort (O(n^2) average/worst case, O(n) best case)
    *   Merge Sort (O(n log n) average/worst case)
*   **Basic Testing:** Includes a cell to run the sorts on a small predefined array and print the results.
*   **Performance Measurement:** Uses `time.perf_counter()` to measure the execution time of each algorithm on pre-generated, shuffled arrays of increasing sizes. Uses caching to avoid re-calculating times unnecessarily.
*   **Interactive Visualization:**
    *   Plots execution time vs. array size for each algorithm using `matplotlib`.
    *   Uses `ipywidgets` (Checkbox, IntSlider) to allow users to:
        *   Show or hide the performance plot.
        *   Adjust the maximum array size included in the plot dynamically.

## Requirements

*   Python 3.x
*   A Jupyter Notebook environment (e.g., Jupyter Lab, Jupyter Notebook, Google Colab, VS Code with Jupyter extension).
*   Required Python libraries:
    *   `matplotlib` (for plotting)
    *   `ipywidgets` (for interactive controls - ensure it's enabled in your Jupyter environment)

## How to Use

1.  **Open Notebook:** Launch your Jupyter environment and open `sorts.ipynb`.
2.  **Run Cells:** Execute the cells sequentially from top to bottom.
    *   The initial cells define the sorting functions (`bubble_sort`, `insertion_sort`, `merge_sort`, `merge`).
    *   A test cell demonstrates the sorts on a small array.
    *   The final code cell sets up and runs the performance timing and interactive plotting.
3.  **Interact with Plot:** Once the final cell is run, you will see a checkbox ("Show Plot") and a slider ("Max Array Size").
    *   Ensure the checkbox is ticked to view the plot.
    *   Move the slider to change the range of array sizes plotted (up to 3500). The plot will update automatically.

## Notes

*   The timing measurements can be affected by system load and other factors. Occasional outliers in the plot might occur; rerunning the timing cell usually resolves this.
*   The notebook pre-generates fixed random arrays for each size to ensure consistent comparisons between algorithms on the *same* input data for a given run.

## File Structure

*   `sorts.ipynb`: The Jupyter Notebook containing all code, explanations, and outputs.

## License

MIT License

## Author

Andrew Obwocha
