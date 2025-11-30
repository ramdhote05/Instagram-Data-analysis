# Projects
Python-based project built to demonstrate clean coding practices, modular design, and real-world problem solving using modern Python libraries. 

Instagram Profile Analysis

A Python-based data analysis project that parses and analyzes Instagram profile data from Bangalore's tech community which is learn from @codewithharry data science course. The notebook extracts key metrics including posts, followers, following counts, and profile categories, then generates interactive visualizations.

Project Overview:-

This project processes raw Instagram profile data from a text file and converts it into structured JSON format for analysis. It identifies top performers, analyzes user categories, and creates an interactive dashboard showcasing various metrics across 100+ Instagram profiles from Bangalore's tech ecosystem.

Features:-

- **Data Parsing**: Converts unstructured text data into clean, structured JSON format
- **Metric Extraction**: Parses username, posts, followers, following, bio, and account type
- **Statistical Analysis**: Identifies profiles with maximum posts, followers, and following
- **Category Analysis**: Categorizes profiles into 34 distinct types (Developer, Media, Community, etc.)
- **Interactive Dashboard**: Generates HTML dashboard with top 10 rankings and category distribution

Dependencies:-

-----Install the required packages before running the notebook:

pip install pandas numpy matplotlib plotly


**Required Libraries:**
- `pandas` - Data manipulation and analysis
- `numpy` - Numerical operations
- `json` - JSON file handling (built-in)
- `matplotlib.pyplot` - Basic plotting
- `plotly.express` and `plotly.graph_objects` - Interactive visualizations

Data Source:-

The project requires a `finaldata.txt` file containing Instagram profile data in the following format :

username
XXX posts
XXX followers
XXX following
Full Name
Account Type
Bio text...


**Data Format Notes:**
- Each profile should be separated by double newlines (`\n\n`)
- Follower/following counts support K (thousands) and M (millions) suffixes
- Posts must be numeric values
- Account type and bio are optional fields

How to Run:-

1. **Prepare your data file**: Place `finaldata.txt` in the same directory as the notebook
2. **Open the notebook**: Launch Jupyter Lab/Notebook

jupyter notebook openai-instagram-analysis.ipynb
3. **Run all cells**: Execute cells sequentially or use "Run All" from the menu
4. **View outputs**: Check console outputs for statistics and open `instagram_dashboard.html` for interactive visualizations

Output Files:-

**data.json**
- Structured JSON file containing all parsed profiles with fields:
- `username`: Instagram handle
- `no_of_posts`: Total post count
- `no_of_followers`: Follower count (numeric)
- `no_of_following`: Following count (numeric)
- `name`: Display name
- `type_of_page`: Account category
- `bio`: Profile biography

**instagram_dashboard.html**
- Interactive Plotly dashboard featuring:
- Top 10 profiles by posts
- Top 10 profiles by followers
- Top 10 profiles by following
- Category distribution pie chart

Key Findings:-

Based on the analysis of Bangalore tech community profiles :

- **Most Active**: `startuphub_blr` with 2,300 posts
- **Highest Followers**: `anujsinghal` with 681,000 followers
- **Most Following**: `bangaloretechbro` with 890 accounts followed
- **Categories**: 34 unique account types including Developer, Media, Community, Blogger, Educator, and Tech Creator
- **Community Focus**: Strong representation of tech communities, startups, and coding education accounts

Analysis Insights:-

The dataset reveals Bangalore's vibrant tech ecosystem with profiles spanning software engineers, startup founders, tech media, coding communities, and café culture enthusiasts. Location tags frequently mention areas like Koramangala, HSR Layout, Indiranagar, and Whitefield .

Project Structure:-


├── openai-instagram-analysis.ipynb # Main analysis notebook
├── finaldata.txt # Raw input data (required)
├── data.json # Parsed output (generated)
├── instagram_dashboard.html # Visualization dashboard (generated)
└── README.md # This file


Author:-

Created as part of data analysis and visualization portfolio projects which is learn from @codewithharry data science course.

License:-

This project is for educational and portfolio purposes.

