# Aggregation and Analysis of Diffusion of Microfinance Data

<a href = "http://nbviewer.jupyter.org/github/aboomer07/Complex_Networks/blob/master/Network_Analysis.ipynb?flush_cache=False">Link to Notebook Viewer</a>

## Explanation and Sources
*All data comes from the Harvard Dataverse website. The paper is cited below:*

*Banerjee, Abhijit; Chandrasekhar, Arun G.; Duflo, Esther; Jackson, Matthew O., 2013, "The Diffusion of Microfinance", hdl:1902.1/21538, Harvard Dataverse, V9*

**The paper studies how microfinance is diffused through social networks within villages in rural India. People's everyday activity's and interactions were coded into adjacency matrices so that their interactions can be studied and analyzed.**

The notebook below is, for now, an exploratory analysis of this data. I start off by taking the large number of files (75 villages, several interaction types, and Person/House type, and storing all these files into dictionaries of dataframes that can be called by their adjusted filenames. This helped with organization, as I also built a dataframe of file names corresponding to the village, activity, and type I wanted to look at.

The exploration so far, which I am working on finishing, involves calculating a variety of complex network metrics for each village and interaction type, that can be put into its own dataframe. The thought behind this is that I can pair this with the demographic data for each person/house and see how well the demographic data given can predict various network characteristics/hierarchies/positions within the networks.

For example, one potential (unproven outcome) would be that households with roof type 3 are more likely to have (or do have) a higher betweenness centrality than other households in the village. Once the functions are defined to organize this data, I can train some machine learning algorithms on the data to see how well this fits.
