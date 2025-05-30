Replication Package for 
"Does Carrying News Increase Engagement with Non-News Content on Social Media Platforms?"
Authors: Yu Song; Puneet Manchanda

This README outlines the contents and usage instructions for the replication package associated with the study. 

================================================================================
DATA USAGE AND COMPLIANCE
================================================================================
In compliance with Data User Agreements, we are unable to publicly share the original dataset used in our study. 
We provide synthetic data instead:
- A randomly sampled subset of Facebook posts and accounts
- Noise added to protect identities

================================================================================
DIRECTORY STRUCTURE
================================================================================
/synthetic_data/   →  Contains datasets used for regressions and figures  
/figures/          →  Stores generated figures in .jpg format  
/tables/           →  Stores generated tables in .tex format  

================================================================================
FILE DESCRIPTIONS
================================================================================
user_engagement.R  
   - Generates results related to non-news user engagement  
   - Reads 'user_engagement.csv' from the /synthetic_data/ folder  

content_generation.R  
   - Generates results related to content generation by non-news accounts  
   - Reads 'content_generation.csv' from the /synthetic_data/ folder  

================================================================================
FIGURES
================================================================================
Purpose:  
- Generates all figures from the main paper, including:  
  • Follower distribution  
  • Daily engagement patterns  
  • Leads-and-lags analysis  

Output:  
- Saved as .jpg files in the /figures/ directory  

================================================================================
TABLES
================================================================================
Purpose:  
- Generates all tables from the main paper, including:  
  • Summary statistics  
  • Regression results  

Output:  
- Saved as .tex files in the /tables/ directory  

================================================================================
SOFTWARE REQUIREMENTS
================================================================================
R version 4.3.1 or later  

Required R packages:  
  • data.table  
  • dplyr  
  • fixest  
  • ggplot2  
  • xtable  

Install via:  
```r
install.packages(c("data.table", "dplyr", "fixest", "ggplot2", "xtable"))

================================================================================
REPLICATION NOTES
================================================================================

This replication package complies with Marketing Science policies:

• **Data Privacy**: All proprietary data have been masked or substituted with synthetic versions.  
  As a result, reproduced figures/tables may differ slightly from those in the published paper.

• **Usage Restrictions**: Data provided are for replication purposes only.  
  Commercial or unauthorized usage is prohibited.

================================================================================
USAGE INSTRUCTIONS
================================================================================

To replicate all figures and tables:

1. Open R and set the working directory to the project root.  
2. Run `user_engagement.R` and `content_generation.R` to generate all results.
