# Clustering-of-scientific-articles
Extraction of knowledge from the text for the purpose of discovering themes, it consists of processing data and building matrixes, using the graph clustering algorithm "louvrain algorithm". Detection of consensus communities. And create a dashboard containing a descriptive analysis with Qlick vue.




We have a text file containing information on scientific articles published in journals and conferences. This information includes:
- The title of the article,
- The author (s),
- The year of publication,
- Name of the journal (or conference)
- Citations between articles.

Part 1:
1) Download the dataset (DBLP_Subset.txt file on the following link http://up5.fr/yMZbV).
2) Load the text file under python
3) Carry out the data processing (word processing) in order to extract the information separately in the form of a dataframe (figure below).
4) Build the Documents-terms matrix for the titles of the articles as well as for the abstracts. Add an "Id" column representing the document identifier to the matrices
Documents-terms. This column will allow us to link this table to the dataframe containing the information of the articles.
5) Create a dataframe representing the authors and assign each author an identifier "author_id".
6) Build the Documents-authors matrix. Insert an "Id" column representing the document identifier.
These operations are necessary in order to be able to link this information to the "Qlik Sense" tool.
Once these four 'dataframes' have been created:
● A "dataframe" containing article information.
● A "dataframe" containing the document-terms matrix (title and summary).
● A "dataframe" containing the identifiers of the authors.
● A "dataframe" containing the document-author matrix.
Generate the CSV files for these data tables and upload them to a Qlik Sense application, to create a dashboard containing a detailed descriptive analysis of the database
created.

Part 2:
7) Construct the four graphs co-terms (title), co-terms (abstract), co-authors, citations.
8) Carry out clustering using the Louvain algorithm on the four graphs.
Save the results in CSV format so that you can make the link with the previously loaded files.
9) Achieve a consensus between the partitions discovered by the previous clusterings.
Create a second dashboard to analyze the results of clustering.
