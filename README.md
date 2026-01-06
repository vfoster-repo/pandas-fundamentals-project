# Movies and Shows Data Analysis

A comprehensive data analysis project using Python and pandas to explore a dataset of movies and TV shows, including information about cast members, genres, release years, and IMDb ratings.

## Project Overview

This project demonstrates fundamental data analysis skills including:
- Data cleaning and standardization
- Exploratory data analysis (EDA)
- Data filtering and manipulation with pandas
- Custom function development for reusable analysis
- IMDb rating categorization and insights

## Dataset

The analysis uses the `movies_and_shows.csv` dataset, which contains:

| Column | Description |
|--------|-------------|
| `name` | Actor or actress name |
| `character` | Character played |
| `role` | Role type (e.g., ACTOR, DIRECTOR) |
| `title` | Movie or show title |
| `type` | Content type (MOVIE or SHOW) |
| `release_year` | Year of release |
| `genres` | List of genres |
| `imdb_score` | IMDb rating (0-10) |
| `imdb_votes` | Number of IMDb votes |

## Getting Started

### Prerequisites

```bash
python 3.7+
pandas
jupyter notebook (or JupyterLab)
```

### Installation

1. Clone this repository:
```bash
git clone https://github.com/vfoster-code/pandas-fundamentals-project.git
cd pandas-fundamentals-project
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Launch Jupyter Notebook:
```bash
jupyter notebook movies_analysis_project.ipynb
```

Alternatively, you can view the notebook by opening `movies_analysis_project.html` in any web browser for a read-only view of the complete analysis.

## Repository Structure

```
pandas-fundamentals-project/
│
├── README.md
├── requirements.txt
├── index.html
├── movies_analysis_project.ipynb
└── data/
    └── movies_and_shows.csv
```

## Key Features

### 1. Data Cleaning
- Standardized inconsistent column names
- Converted mixed-case headers to lowercase with underscores
- Replaced special characters for consistency

### 2. Custom Functions

#### `get_actors_for_title(title)`
Returns a comma-separated list of all actors for a given movie or show.

```python
get_actors_for_title("Taxi Driver")
# Returns: "Robert De Niro, Jodie Foster, Harvey Keitel, ..."
```

#### `categorize_imdb_score(title)`
Categorizes movies/shows into quality tiers based on IMDb scores:
- **Excellent**: ≥ 9.0
- **Good**: 7.0 - 8.9
- **Average**: 5.0 - 6.9
- **Low**: < 5.0

```python
categorize_imdb_score("The Godfather")
# Returns: "Excellent"
```

#### `filter_by_decade(df, start_year)`
Filters content by decade for time-based analysis.

```python
filter_by_decade(df, 1990)
# Returns DataFrame with all 1990s content
```

## Analysis Highlights

- **Data Quality**: Successfully cleaned and standardized 9 columns
- **Content Coverage**: Analyzed thousands of movies and shows across multiple decades
- **Rating Insights**: Identified highly-rated content and categorization patterns
- **Genre Analysis**: Explored genre distributions and trends

## Skills Demonstrated

- **Python**: pandas, data manipulation, function development
- **Data Cleaning**: Handling inconsistent data formats
- **EDA**: Exploratory analysis and insight generation
- **Problem-Solving**: Creating reusable, modular functions
- **Documentation**: Clear code comments and markdown explanations

## Future Enhancements

Potential areas for expansion:
- [ ] Visualizations with matplotlib/seaborn
- [ ] Genre trend analysis over time
- [ ] Actor performance metrics
- [ ] Correlation analysis between votes and ratings
- [ ] Interactive dashboard with Plotly or Streamlit

## License

This project was completed as part of the TripleTen AI/ML Engineering program.

## Author

**Victor Foster**
- GitHub: [@vfoster-repo](https://github.com/vfoster-repo)
- LinkedIn: [Victor Foster](https://linkedin.com/in/vfoster-connect)
- Email: victorfoster@hotmail.com

## Acknowledgments

- TripleTen  AI/ML Engineering Program Sprint 2 "Working with data in Python"

---

If you found this project helpful, please consider giving it a star!
