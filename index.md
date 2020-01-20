### Welcome to University of Turku cell line name recognition and normalization
The project is a result of collaboration of University of Turku, Gent University and Textimi. The aim is to create corpora that is suitable for training and evaluating machine learning systems to recognize and normalize established cell line names from text. 

### Gellus and CLL Corpora
We created two manually annotated corpora, Gellus and CLL. Gellus is suitable for the training of any machine learning systems in recognizing cell line name mentions while CLL is for evaluating the systems in recognizing the Cellosaurus cell line names.

* [GELLUS](http://bionlp-www.utu.fi/cell-lines/Gellus_corpus.tar.gz)
* [CLL](http://bionlp-www.utu.fi/cell-lines/CLL_corpus.tar.gz)

### Cell line names dictionary
We prepared a dictionary of cell line names derived from the Cellosaurus resource (version 6.5) separating information into synonyms, resources and categories. We also gathered human cancer cell line mutation information from CCLE and Cosmic.

* [Synonyms](http://bionlp-www.utu.fi/cell-lines/cell_line_dictionary_synonyms.tab)
* [Sources](http://bionlp-www.utu.fi/cell-lines/cell_line_dictionary_resources.tab)
* [Categories](http://bionlp-www.utu.fi/cell-lines/cell_line_dictionary_categories.tab)
* [Mutations](http://bionlp-www.utu.fi/cell-lines/cell_line_dictionary_mutations.tab)

### NERsuite model and corpora
We used NERsuite as our machine learning system trained on Gellus corpus and supplemented with cell line name dictionary to achieve state-of-the-art performance. In addition to NERsuite model, we provide the derived corpora used in our studies for those who want to train their own systems.

* [NERsuite model](http://bionlp-www.utu.fi/cell-lines/NERsuite_Gellus_Cellosaurus.m)
* [dictionary](http://bionlp-www.utu.fi/cell-lines/cell_line_dictionary.db): To use this dictionary with NERsuite, you can skip the compiling step (command: nersuite_dic_compiler) and use it directly with command nersuite_dic_tagger.
* [JNPBA-CL](http://bionlp-www.utu.fi/cell-lines/JNLPBA-CL_corpus.tar.gz)
* [CellFinder-CL](http://bionlp-www.utu.fi/cell-lines/CellFinder-CL_corpus.tar.gz)
  
### Tagged and normalized cell line name documents (updated 20 September 2018)
Originally we provided text documents and cell line names annotation in standoff format in roughly 24M documents, including both PubMed abstracts and PMC-Open Access (PMCOA) full texts. 

Since then, there are newly published articles available from those two literature database, currently >27M PubMed abstracts and >2M PMCOA full texts. We instead provided following link to our weekly-update large-scale named entity recognition project, where the cell line annotations and text documents are provided in TEES-xml format.

* [Syntactic parses and named entity recognition for PubMed abstracts and PubMed Central full documents](https://turkunlp.github.io/pubmed_parses/)

### Authors and Contributors
* Suwisa Kaewphan, University of Turku
* Sofie Van Landeghem, Gent University
* Tomoko Ohta, Textimi
* Yves Van de Peer, Gent University
* Filip Ginter, University of Turku
* Sampo Pyysalo, University of Turku 

### Support or Contact
Please contact sukaew@utu.fi or sampo.pyysalo@gmail.com for further information or questions.
