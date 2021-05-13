# Uncovering Momentum

This repository encompasses the notebooks for replicating the results from the paper 
[Uncovering Momentum](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3502301). 
The study explores and explains the source of the momentum premium, 
a long-term ongoing challenge in the financial economics domain. 

The ambitious task is tackled by a systematic divide-and-conquer approach composed of 
top-bottom steps proceeding from the momentum factor into the stock level. The first 
version of the approach is described in the paper available on SSRN and consists of the 
following four steps: dissecting the momentum performance along bull/bear states and 
winners/losers deciles; identifying the unscaled momentum decile as a basic common block 
across alternative momentum strategies; rolling the combined in- and out-of-sample 
analysis; and clustering momentum decile time series. Then, the subsequent research 
updated the latest step with the selection of characteristic-related anomalies and 
tracing their transition through the ranking and holding intervals as described in the 
Towards Data Science article 
“[Uncovering Momentum with Rolling Intertemporal Analysis](https://towardsdatascience.com/uncovering-momentum-effect-with-rolling-intertemporal-analysis-36eedc1d8a96)”. 

**To summarize, the study identified the 2010-2019 momentum effect as the sampling of high 
volatility growth stocks**.

The initial approach presented in the paper was conducted within the Quantopian 
environment and then transitioned to the open-source platform based on the 
[Zipline](https://github.com/quantopian/zipline) algorithmic trading library and Flounder 
extensions. The corresponding notebooks in this repository align with each step of 
the applied approach as follows:

- **Section 1**: Dissecting Momentum Performance, [UM.s1.ipynb](./UM.s1.ipynb)

	The section demonstrates the heterogeneous behavior of momentum across bull/bear market 
states and winners/losers deciles and suggests that each dissected case can be associated 
with different processes, hence requiring independent evaluation.

- **Section 2**: Momentum Decile as a Common Block Across Momentum Strategies

	The section detaches the volatility scaling component from the time series momentum 
portfolio and identifies the momentum decile as a basic common block across alternative 
conventional and time-series strategies .

- **Section 3**: Applying the Rolling Intertemporal Analysis to Momentum Decile

	The section combines the ranking and holding intervals within the rolling intertemporal 
analysis and switches the focus of previous research on momentum premium from the holding 
period to the analysis of the transition processes.

- **Section 4**: Explaining the Momentum Effect

	The section progresses to the stock level by dividing momentum deciles into portfolios 
based on fundamental and technical characteristics and then applying the rolling 
event-oriented intertemporal analysis for identifying anomalies contributing to the 
premium. The results transparently and completely explain the momentum premium for 
2010-2019 as the sampling of high volatility growth stocks. 