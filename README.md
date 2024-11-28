# Aggregate volatility

Code and data attached to an upcoming article on the empirics of aggregate fluctuations by Magermann, Lafond, Lumma.
The authors of the upcoming article gratefully acknowledge the ONS-Turing Strategic partnership for funding.
The authors would also like to thank the ONS-Turing Strategic Partnership team, in particular Gesine Reinert, Mihai Cucuringu, Kerstin Hotte and Anastasia Mantziou, for useful comments and economic insights to this project. We also thank Keith Lai, Alex Holmes, Dragos Cozma and Nathan Williams from the Office for National Statistics for providing an experimental version of the data, as well as for providing data insights. 


The 'Data_Cleaning' folder contains the code that is used to transform the raw data obtained through the ONS-Turing partnership. In particular, this involves
- Taking the raw data which comes in a payment network format (i.e. sources correspond to sources of payment flows) and transform it into a production network formalism (where sources now correspond to sources of goods being produced)
- Removing the non-market and industries with different input-output characteristics than national account data. This involves removing industries with the following SIC-2 codes: 45, 46, 47, 64, 65, 66 and 84 and above.
- Merge industries that would have zero aggregate output in at least one month with closely related industries.

The 'Factor_Analysis' folder contains the code that is used to
- compute unfiltered and filtered growth rates.
- perform the factor analysis on filtered and unfiltered growth rates.
- compute aggregate quantities of industry-level filtered and unfiltered growth rates, as well as of their common and idiosyncratic modes.
- compute contributions to aggregate volatility.

The 'Time_Varying_Volatility' folder contains an analysis of the variables contributing to changes in volatility. 
Changes in volatility can be due to changes in the network structure, changes in the shares or changes in the covariance matrix of growth rates.
