# PerfoRank: Cluster-Based Performance Ranking for Improved Performance Evaluation and Estimation in Professional Cycling

Current cycling analytics solutions do not account for the race course profile or the level of the competition. Therefore, this paper develops a unique two-stage clustering-based ranking approach for rider evaluation. Initially, races are segmented into coherent clusters based upon elevation and road surface type. Subsequently, underlying skill levels are determined per cluster through the observed race results using the TrueSkill algorithm which allows to model multi-entrant competitions. The results indicate that our approach results into clusters which match the commonly known specializations in road cycling. The ranking methodology results in skill ratings which enable the identification of specialization and can be used in downstream tasks. Our results show that the proposed rankings drastically improve race outcome estimation when adding these rankings as features to the current prediction models. Manuscript forthcoming in *Machine Learning*.

The FEClustering.ipynb notebook is used to cluster all professional cycling races into coherent clusters using various clustering algoirthms, and evaluated on an annotated valuation set, as discussed in the manuscript. Moreover, it also includes the code for the feature engineering of the climb count and location features, as this may be less straightforward.

The TrueSkill.ipynb notebook contains the code to calculate the three ranking methods, and its comparison.

Finally, the CaseStudy.ipynb notebook contains the code to do the downstream race outcome estimation benchmark study.

All data can be found within this GitHub repository, besides some large files. As these files were too large to upload to GitHub, we uploaded these to figshare: https://figshare.com/articles/dataset/PerfoRank_Data/25117451 
