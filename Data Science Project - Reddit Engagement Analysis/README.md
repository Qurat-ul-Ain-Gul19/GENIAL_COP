# Reddit Community Engagement Analysis

## Project Overview

This project investigates engagement patterns across three technology and science-oriented subreddits (r/technology, r/science, and r/Futurology) to understand how different communities interact with content. By analyzing post scores and comment counts, the project reveals distinct engagement hierarchies and correlation patterns that characterize each community's discussion culture.

The analysis addresses the research question: **"How does post engagement—measured by upvotes (score) and comments—differ across technology and science-oriented subreddits?"**

## Setup Instructions

### Prerequisites
- Python 3.8+
- Reddit account with developer app credentials
- Required packages: `pandas`, `requests`, `matplotlib`, `seaborn`, `python-dotenv`

### Quick Start
1. Clone this repository
2. Install dependencies: `pip install -r requirements.txt`
3. Create Reddit developer app at https://www.reddit.com/prefs/apps
4. Set environment variables or use .env file:
   ```
   REDDIT_CLIENT_ID=your_client_id
   REDDIT_CLIENT_SECRET=your_client_secret
   REDDIT_USER_AGENT=ProjectName/1.0 by YourUsername
   ```
5. Run notebooks sequentially:
   - `NB01 - Data Gathering.ipynb` → Collects data and creates database
   - `NB02 - Exploratory Data Analysis.ipynb` → Analyzes data and generates visualizations

### Google Colab Instructions
All notebooks are Colab-compatible. Mount your Google Drive and use `getpass` for secure credential entry when prompted.

## Project Structure
```
├── data/
│   └── database.db              # SQLite database with Reddit data
├── figures/                     # Generated visualizations
├── notebooks/
│   ├── NB01 - Data Gathering.ipynb
│   └── NB02 - Exploratory Data Analysis.ipynb
├── README.md                    # This file
├── REPORT.md                    # Analysis findings and insights
├── requirements.txt             # Python dependencies
└── .gitignore                   # Git ignore configuration
```

## Key Findings

The analysis reveals that r/technology significantly outperforms r/science and r/Futurology in both average post scores (~2,700 vs ~2,200 vs ~1,000) and comment counts (~190 vs ~150 vs ~105). A positive correlation between scores and comments exists across all subreddits, though each community exhibits unique engagement patterns reflecting their content focus and discussion culture.

## Acknowledgements

- **Reddit API** for providing programmatic access to community data
- **DS105 Course Team** at LSE for foundational data science concepts and project framework
- **Python Community** for powerful data analysis libraries (pandas, matplotlib, seaborn)
- **Stack Overflow** for troubleshooting support during development
- **Claude AI** for code assistance and debugging support throughout the project
- **OpenAI's ChatGPT** for code assiatance, debugging and report formulation

## References

- Reddit API Documentation. (2024). *Reddit Developer Platform*. https://www.reddit.com/dev/api
- McKinney, W. (2022). *Python for Data Analysis* (3rd ed.). O'Reilly Media.
- Wickham, H., & Grolemund, G. (2017). *R for Data Science*. O'Reilly Media. [Concepts adapted to Python]
- Hunter, J. D. (2007). Matplotlib: A 2D graphics environment. *Computing in Science & Engineering*, 9(3), 90-95.
- LSE DS105 Course Materials. (2024). *Data for Data Science*. London School of Economics.

---

**Author**: Qurat-ul-ain Gul
**Course**: DS105 - Data for Data Science  
**Institution**: London School of Economics  
**Date**: 14th June, 2024
