
# Setup
Download `influence_data.csv` at kaggle  [here](https://www.kaggle.com/ironicninja/icm-problem-d).

Find the arrows tool [here](http://www.apcjones.com/arrows/).

# Import
Change line 1 of `load.cql` to point to the location of your `influence_data.csv` file.
        
   Windows path: `file:///influence_data.csv`

I have cleaned up a little bit of data in it. `file:///influence_data.csv`
    
This section contains information on all the clauses in the [Cypher query language](https://neo4j.com/docs/cypher-manual/current/clauses/).
     
     LOAD CSV WITH HEADERS FROM "filepath" AS row
      WITH row WHERE row.ID IS NOT NULL
      MERGE row

 # Algorithms
This analysis uses [Centrality Algorithms](https://neo4j.com/docs/graph-data-science/current/algorithms/centrality/)
