# ComplexNetworks2019
Material for lectures at Fields institute, August 2019:

Web page: http://128.100.216.27/activities/19-20/complex-networks

Poster: http://128.100.216.27/sites/default/files/CQAM_SummerSchoolDataScienceTools%2BTechniquesInModellingComplexNetworks.pdf

## Useful links:

I will illustrate the talks using Jupyter notebooks and Python 3 code:
https://www.anaconda.com/distribution/

I will use stardard packages (numpy, pandas ..) plus igraph, networkx and umap.

##conda install -c conda-forge python-igraph 

Python igraph documentation: https://igraph.org/python/

## Reference papers and code:

ECG papers: https://rdcu.be/bLn9i and https://arxiv.org/abs/1809.05578

ECG code: https://codeocean.com/capsule/3898939/tree/v1

Graph clustering comparison measures paper: https://arxiv.org/abs/1806.11494

Graph clustering comparison measure code: https://codeocean.com/capsule/0712485/tree/v1

Graph embedding comparison paper: https://arxiv.org/abs/1906.04562

Hypergraph modularity paper: https://arxiv.org/abs/1810.04816

Tutorial on spectral clustering: http://www.tml.cs.uni-tuebingen.de/team/luxburg/publications/Luxburg07_tutorial.pdf

Regularization framework for graph data: https://www.researchgate.net/publication/41781181_A_Regularization_Framework_for_Learning_from_Graph_Data

Learning with Hypergraphs: https://papers.nips.cc/paper/3128-learning-with-hypergraphs-clustering-classification-and-embedding.pdf

Chung-Lu model: https://e-reports-ext.llnl.gov/pdf/802505.pdf

Topological features: Orman et al., https://arxiv.org/abs/1206.4987

Z. Yang et al, A Comparative Analysis of Community Detection Algorithms on Artificial Networks, Scientific Reports volume 6, Article number: 30750 (2016) https://www.nature.com/articles/srep30750


## Datasets

Football dataset: M. Girvan and M. E. J. Newman, Community structure in social and biological networks, Proc. Natl. Acad. Sci. USA 99, 7821-7826 (2002). http://www-personal.umich.edu/~mejn/netdata/

Karate Club dataset:  Zachary, W. W. An information flow model for conflict and fission in small groups. Journal of Anthropological Research 33, 452-473 (1977). http://www-personal.umich.edu/~mejn/netdata/

LFR generator: https://github.com/eXascaleInfolab/LFR-Benchmark_UndirWeightOvp

YouTube and other datasets: J. Leskovec, A. Krevl. SNAP Datasets: Stanford Large Network Dataset Colection, http://snap.stanford.edu/data/

## networkx

networkx graphs can be transformed into igraph format via:
```
import networkx as nx, igraph as ig
# create networkx graph
g1 = nx.planted_partition_graph(5, 5, 0.9, 0.1)
# convert and plot
g = ig.Graph(directed=False)
g.add_vertices(g1.nodes())
g.add_edges(g1.edges())
```
Upcoming book with networkx examples: https://github.com/CambridgeUniversityPress/FirstCourseNetworkScience

