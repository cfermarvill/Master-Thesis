# Master-Thesis

## Analysis of information dissemination in subreddits during the Russia-Ukraine Conflict

### Author: Fernanda Martín Villaescusa

All the necessary scripts for the complete replication of the analysis carried out in the master thesis on the dissemination of information on reddit.

To collect the data, we utilised a downloader tool1 that retrieves the data from Reddit via its official API you can find it [here.](https://github.com/ArthurHeitmann/arctic_shift)

The data is downloaded in JSON format, then cleaned and filtered with the JQ tool. However, the JSON files were too heavy, so R didn't allow us to read them, that's why these files are transformed to RSD one by one. You can replicate this process with your own JSONs with the script of [**Read the data.Rmd**](https://github.com/cfermarvill/Master-Thesis/blob/main/Read%20The%20Data.Rmd).

In the [**PreProcessing.Rmd**](https://github.com/cfermarvill/Master-Thesis/blob/main/PreProcessing.Rmd) script, all previously obtained RSDs are read, to finally have a clean database for the analysis. This resulting database can be found on google drive ‘[**OK_final_data.rsd**](https://drive.google.com/file/d/1VPCLUTZxWtgbm6PLShoTQdGgu-WCEFGu/view?usp=drive_link).

With the **OK_final_data** database, the entire network analysis carried out for the research on the consumption of information sources on Reddit is fully replicable. This complete and detailed analysis can be found in [**Analysis Network.Rmd**](https://github.com/cfermarvill/Master-Thesis/blob/main/Analysis%20Network.Rmd).

In addition to this network analysis, a content analysis was also performed by constructing word clouds with the titles of the posts of the subreddits being examined. For the replication of this analysis in [**Word Cloud.Rmd**](https://github.com/cfermarvill/Master-Thesis/blob/main/Word%20Cloud.Rmd) it is necessary to have a clean database with the titles as [**title.rds**](https://github.com/cfermarvill/Master-Thesis/blob/main/title.rds), which was also generated in the [**Read The Data.Rmd**](https://github.com/cfermarvill/Master-Thesis/blob/main/Read%20The%20Data.Rmd) script.
