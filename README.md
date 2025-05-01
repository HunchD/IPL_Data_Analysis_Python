# IPL Match Insights


## Overview
**IPL Match Insights** is a data analysis project that visualizes various aspects of the IPL match between Royal Challengers Bengaluru (RCB) and Delhi Capitals (DC) on April 10th 2025. Implemented in a Jupyter Notebook using Python, Pandas, Matplotlib, and Seaborn, the project includes multiple visualizations such as top scorers, run distribution per over, significant partnerships, bowling economy rates, wicket fall timelines, extras breakdown, and scoring shot distribution. This project showcases data manipulation, visualization, and cricket analytics skills, making it an ideal addition to a data science portfolio for sports analytics enthusiasts, data scientists, or recruiters.

## Dataset
The project uses a CSV file [RCB_vs_DC_April_10](/data/RCB_vs_DC_April_10.csv), sourced from [Statso](https://statso.io/ipl-2025-match-dataset/), containing ball-by-ball data for the RCB vs DC IPL match. Key columns include:
- `team`: Batting team (Royal Challengers Bengaluru or Delhi Capitals).
- `over`: Over number (0 to 19).
- `batter`: Player batting.
- `bowler`: Player bowling.
- `non_striker`: Player at the non-striker’s end.
- `runs_batter`: Runs scored by the batter (0, 1, 2, 4, 6).
- `runs_extras`: Runs from extras (e.g., wides).
- `runs_total`: Total runs scored on the delivery.
- `extras_type`: Type of extra (e.g., wides).
- `wicket_kind`: Type of wicket (if any, e.g., caught).
- `player_out`: Player dismissed (if any).
- `fielders`: Fielders involved in a dismissal (if any).


## Installation
To run the Jupyter Notebook locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/HunchD/IPL-Data-Analysis-Python.git
   cd IPL-Match-Insights
   ```

2. **Set Up a Python Environment** (recommended: Python 3.12.7):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   Install the required Python libraries using the provided `requirements.txt`:
   ```bash
   pip install -r requirements.txt
   ```

   The `requirements.txt` includes:
   ```
   pandas==2.2.2
   matplotlib==3.8.4
   seaborn==0.13.2
   jupyter==1.0.0
   ```

4. **Install Jupyter Notebook** (if not already installed):
   ```bash
   pip install jupyter
   ```

5. **Add the Dataset**:
   Place the `RCB_vs_DC_April_10.csv` file in the `data` directory. Ensure the notebook’s file path (`pd.read_csv("data/RCB_vs_DC_April_10.csv")`) matches this location. If using a different path, update the notebook accordingly.

## Usage
The project is contained in a single Jupyter Notebook (`notebooks/IPL_Analysis.ipynb`). To run the analysis and generate the plots:

1. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```
   This opens a browser window. Navigate to the `notebooks` directory, open `IPL_Analysis.ipynb`, and run it.

2. **Run the Notebook**:
   - Execute all cells in sequence (Cell > Run All) to load the dataset and generate all visualizations.
   - Alternatively, run individual cells to step through the data loading and visualization.
   - Plots are saved automatically (e.g., `scoring_shot_distribution_rcb_vs_dc.png`).

3. **Output**:
   - The notebook displays multiple plots including top scorers, run distribution per over, significant partnerships, bowling economy rates, wicket fall timelines, extras breakdown, and scoring shot distribution.
   - Saved plots are high-resolution PNGs suitable for reports or portfolios.

### Example Outputs
- **Top Scorers**: A bar chart comparing the total runs scored by top players from RCB and DC.
- **Run Distribution Per Over**: A line plot showing runs scored per over for both teams.
- **Significant Partnership Analysis**: A bar chart highlighting partnerships scoring 10+ runs for RCB and DC.
- **Bowling Economy Rates**: A bar chart comparing the economy rates of bowlers from both teams.
- **Wicket Fall Timeline**: A step plot showing the cumulative wickets lost per over for RCB and DC.
- **Extras Breakdown**: A stacked bar chart showing the distribution of wides, legbyes, and no-balls for each team.
- **Scoring Shot Distribution**: A stacked bar plot comparing the number of deliveries for each run type (0, 1, 2, 4, 6) for RCB and DC.


## Project Structure
```
IPL-Match-Insights/
├── data/
│   └── RCB_vs_DC_April_10.csv           # Dataset 
├── notebooks/
│   └── IPL_Analysis.ipynb               # Jupyter Notebook with all analyses
├── figures/
│   ├── scoring_shot_distribution_rcb_vs_dc.png  # Generated plot
│   ├── top_scorers_rcb_vs_dc.png                 # Generated plot
│   ├── run_distribution_per_over_rcb_vs_dc.png   # Generated plot
│   ├── significant_partnerships_rcb_vs_dc.png    # Generated plot
│   ├── bowling_economy_rates_rcb_vs_dc.png       # Generated plot
│   ├── wicket_fall_timeline_rcb_vs_dc.png        # Generated plot
│   └── extras_breakdown_rcb_vs_dc.png            # Generated plot
├── requirements.txt                     # Python dependencies
├── README.md                            # Project documentation
```

## Notebook Structure
The `notebooks/IPL_Analysis.ipynb` notebook is organized as follows:
1. **Setup**: Import libraries (Pandas, Matplotlib, Seaborn) and load the dataset from `data/RCB_vs_DC_April_10.csv`.
2. **Analyses**:
   - **Top Scorers**: Extract and visualize the total runs scored by top players from each team.
   - **Run Distribution Per Over**: Calculate and plot runs scored per over for RCB and DC.
   - **Significant Partnership Analysis**: Identify and visualize partnerships scoring 10+ runs.
   - **Bowling Economy Rates**: Compute and plot the economy rates of bowlers from both teams.
   - **Wicket Fall Timeline**: Track and visualize cumulative wickets lost per over.
   - **Extras Breakdown**: Analyze and plot the distribution of wides, legbyes, and no-balls.
   - **Scoring Shot Distribution**: Group and visualize the frequency of runs scored (0, 1, 2, 4, 6) per team.

Each cell includes:
- Code for data processing or visualization.
- Minimal comments (users can add markdown cells for clarity).
- Final plots displayed inline and saved to the `figures` directory.

## Analysis
The project provides a comprehensive analysis of the RCB vs DC match through multiple visualizations:
- **Top Scorers**: Identifies key performers, with KL Rahul leading Delhi Capitals and PD Salt leading Royal Challengers Bengaluru.
- **Run Distribution Per Over**: Highlights scoring patterns, with peaks indicating aggressive phases (e.g., powerplay or death overs).
- **Significant Partnerships**: Shows impactful batting pairs, with KL Rahul-T Stubbs (DC) and PD Salt-V Kohli (RCB) standing out.
- **Bowling Economy Rates**: Compares bowler effectiveness, with LS Livingstone and MA Starc showing higher economy rates.
- **Wicket Fall Timeline**: Tracks batting stability, with RCB losing more wickets later in the innings.
- **Extras Breakdown**: Reveals extra run contributions, with Delhi Capitals relying more on wides.
- **Scoring Shot Distribution**: Quantifies batting aggression, with RCB showing a higher proportion of 4s and 6s.

## Conclusions
The analyses reveal key insights into the RCB vs DC match:
- **Top Scorers**: KL Rahul (DC) and PD Salt (RCB) were the standout batters, driving their teams’ totals.
- **Run Distribution**: Both teams had fluctuating scoring rates, with RCB peaking early and DC finishing strongly.
- **Partnerships**: DC’s KL Rahul-T Stubbs partnership was more significant, contributing to their stability.
- **Bowling**: RCB bowlers like LS Livingstone faced challenges, while DC maintained tighter control overall.
- **Wickets**: RCB’s late wicket losses suggest a collapse, contrasting with DC’s more even distribution.
- **Extras**: DC’s reliance on wides indicates bowling inconsistency, while RCB balanced extras across types.
- **Scoring Shots**: RCB’s higher 4s and 6s reflect an aggressive approach, while DC relied on singles and twos.

This analysis is valuable for:
- **Coaches and Analysts**: To assess player performance, bowling strategies, and batting stability.
- **Fans and Commentators**: To understand match dynamics and key moments.
- **Data Scientists**: To demonstrate proficiency in multi-faceted sports analytics.

## Future Improvements
- **Additional Analyses**: Player strike rates, bowler wicket charts, or heatmaps of scoring zones.
- **Interactive Visualizations**: Use Plotly for interactive dashboards.
- **Automation**: Support analysis for multiple matches.
- **Streamlit App**: Create a web interface for exploring insights.


---

This project was developed as part of a data analyst portfolio to demonstrate expertise in Python, data analysis, visualization, and sports analytics. Explore the notebook to dive into IPL match insights!
