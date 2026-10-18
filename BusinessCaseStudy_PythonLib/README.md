# 🎬 Movie & Director Data Analysis Using Python and Pandas

## 📌 Project Overview

This project is a hands-on business case study focused on analyzing movie and director datasets using Python and Pandas.

The goal was to practice data manipulation, filtering, aggregation, and merging techniques by solving practical questions using movie-related data.

Through this exercise, I strengthened my understanding of how Python libraries can be used to explore datasets and extract meaningful information.

## 🎯 Objectives

- Explore and understand movie and director datasets.
- Filter records based on specific conditions.
- Analyze movie and director information.
- Combine multiple datasets to retrieve relevant information.
- Write reusable functions to solve data analysis problems.

## 🛠️ Technologies Used

- **Python** — Programming language
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical computing
- **Jupyter Notebook** — Interactive coding and analysis

## 📂 Project Structure

```text
BusinessCaseStudy/
│
├── BusinessCaseStudy_PythonLib.ipynb
├── movies.csv
├── directors.csv
└── README.md
```

*Note: The CSV files should be included in the repository if you want users to run the notebook without downloading them separately.*

## 📊 Key Concepts Covered

### 1. Data Exploration
- Loading CSV files into Pandas DataFrames.
- Inspecting records using `head()` and understanding dataset structure.

### 2. Data Cleaning and Manipulation
- Selecting and removing columns.
- Filtering records using conditions.
- Working with movie release years, months, and days.

### 3. Data Analysis
- Using `groupby()` to summarize data.
- Using `value_counts()` to analyze category frequencies.
- Using `nunique()` to count distinct values.
- Exploring director information, including gender distribution.

### 4. DataFrame Merging
- Combining movie and director datasets using `merge()`.
- Retrieving director information for a particular movie, such as *Spider-Man 3*.

### 5. Reusable Functions
- Creating a function to retrieve movies directed by a specified director within a given year range.
- Practicing conditional filtering and handling cases where a director is not found.

## 💻 Getting Started

### Prerequisites

Make sure Python and Jupyter Notebook are installed on your system.

Install the required libraries:

```bash
pip install pandas numpy jupyter
```

### Run the Project

1. Clone this repository:

   ```bash
   git clone <your-github-repository-url>
   ```

2. Navigate to the project directory:

   ```bash
   cd BusinessCaseStudy
   ```

3. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

4. Open `BusinessCaseStudy_PythonLib.ipynb` and execute the cells.

**Dataset note:** The notebook currently uses Google Drive download commands to retrieve the CSV files. If you include the datasets locally, update the notebook to load `movies.csv` and `directors.csv` directly from the project directory.

## 📚 Key Learnings

This case study helped me gain practical experience with:

- Working with real-world-style tabular datasets.
- Applying Pandas operations to solve specific questions.
- Understanding the relationship between datasets and joining them using common identifiers.
- Breaking down data analysis problems into smaller steps.
- Writing reusable and readable Python code.

## 🚀 Conclusion

This project was a valuable step in strengthening my Python and Pandas fundamentals through practical problem-solving. It helped me understand how data exploration, filtering, aggregation, and merging can work together to answer data-related questions.

I plan to continue building on these skills by solving more case studies and applying data analysis techniques to increasingly complex datasets.

## 🔗 Connect

Thank you for checking out my project! Feedback and suggestions are always welcome.

