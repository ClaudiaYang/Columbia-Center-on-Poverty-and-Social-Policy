## Project Overview:
This project is about exploring new ways to visualize the results from Columbia Center of Policy and Social Policy simulation tool, focusing on SNAP scenarios. The goal is to make complex metrics (like poverty rates, income change, and people lifted out of poverty) easier to interpret and more engaging for advocates, policymakers, and researchers. We are working towards a set of prototype visuals and identify which approaches to develop further. 

## Repository Structure
This repository is built as a Quarto Book, organizing the analysis into weekly design sprints:

index.qmd: Project landing page and executive summary.

Week_1.qmd: Initial exploration in visualizing poverty metrics' changes.

Week_2.qmd: Aggregate poverty metrics and visualize demographic categories.

Week_3.qmd: Revise designs that are moving forward, finetune the labeling, colors, and emphasize storytelling value. Storyboard building.

Week_4.qmd: Aggregated summary visualization and interactive effect analysis using mock dataset.

conclusion.qmd: Final synthesis, limitations, and future roadmap.

cpsp_simulation_data.csv: dataset for changes in poverty metrics

demographic_data.csv: demographic dataset


## Technology and Packages
R Language: Core statistical computing.

Quarto: For reproducible reporting and website generation.

Tidyverse: The primary ecosystem used for data science:

dplyr: Used for data manipulation, calculating reduction deltas, and filtering demographic groups.

tidyr: Used for pivoting data between wide and long formats for ggplot.

readr: For ingesting CSV datasets.

ggplot2: For constructing the static visualization layers.

Plotly: For converting static charts into interactive tooltips.

Viridis: Applied for perceptually uniform, colorblind-safe color scales.


##  How to Reproduce

1. Clone this repository:
   ```bash
   git clone https://github.com/ClaudiaYang/Columbia-Center-on-Poverty-and-Social-Policy.git
   
2. Open the project in RStudio.

3. Install dependencies:
       install.packages(c("tidyverse", "plotly", "quarto", "viridis"))
       
4. Render the website:
    ```r
       quarto::render_book()
    ```



