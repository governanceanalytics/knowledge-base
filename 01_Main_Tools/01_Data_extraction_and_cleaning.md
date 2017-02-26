# Tools and algorithms to process data

## Data Extraction and Cleaning

### Data Cleaning

The objective of data cleaning is to handle the missing data through the identification of the noises and hence to remove outliers and resolve inconsistencies. The data quality is a big issue for the data scientist and business intelligence practitioners. To measure the quality of a data, we usually set up a schema to check the: accuracy, completeness, consistency, timeliness, believability, and interpretability.
The accuracy means whether the data are correct or not, accurate or not. The completeness gives an answer on how recorder is the data. The consistency, checks if the some data splits are modified but some not. The timeliness of data means if the data is timely updated and temporally changed and with which frequency. The believability represents how trustable the data are correct. Finally, the interpretability, gives an idea on how easily the data can be understood.
In the real application use cases, the data is some times incomplete with lacking attributes or values, or simply containing a global aggregate data, which can bring incomplete results. The data can also be noisy, for example a Salary variable that contains a negative value is a noisy outlier value. It can also be inconsistent, by representing contradictory information. For example a person whose birthday is 01/01/2000, at 01/01/2017 should not have an age variable, which equals 10. However, the main problem does still in the missing data. Indeed, working with a complex and large database, with a lot of missing values is a real challenge in data science.
The missing data may have several possible and plausible motifs. For example, it can be caused by an internal problem to the measuring equipment, or the data were simply not entered during the preparation steps, or certain data may not be considered as important during the collection steps, or the users did not register history of the data.
To overcome the problems of missing data, several statistical and mathematical methods have been proposed. As an example, it can be suggested in certain cases to fill automatically with a global constant ‘unknown’ or ‘na’, all the cases where we do have a non-value. The attribute mean is another alternative way to replace a missing value by replacing it with a mean value of the rest of available variables. The problem of noisy data is simpler than the one of missing data. In fact, robust statistical methods can allow us to smooth the data by calculating a mean or a median and thus process the noise regarding these two parameters.

There are a lot of tools dedicated to data cleaning. Among them, we suggest to the reader to choose from the following list:

* [DataWrangler](http://vis.stanford.edu/wrangler/): web-based service from Stanford University's Visualization Group is designed for cleaning and rearranging data so it's in a form that other tools such as a spreadsheet app can use.
*  [Google Refine](http://openrefine.org/): can be described as a spreadsheet on steroids for taking a first look at both text and numerical data.
*	[AnalyticsCanvas](http://analyticscanvas.com/), helps automate Google Analytics and Facebook insights dataflow, connects to various data sources, performs calculations and data transformations, and export data for storage and visualization.
* [analytixBASE](http://www.analytixbase.com/), a self-service analytics software for business users to quickly and easily create reports and analysis without SQL knowledge, using an intuitive and visual work-flow interface.
*	[Astera ReportMiner](http://www.astera.com/reportminer-data-extraction-software) enables users with no technical background to extract & transform data from virtually any report, and map and export data anywhere.
*	[BioComp iManageData](http://www.biocompsystems.com/content/products/analytics/ngo/), Accesses, cleans, filters, converts and transforms data from files, Excel, Oracle, SQL Server, process control systems and more.
*	[Data Ladder](https://dataladder.com/), offering Data Matching, Profiling, deduplication, and Enrichment software and services.
*	[DataFlux](http://support.sas.com/software/products/dfdmstudioserver/), provides Data Management solutions including Data profiling, Data quality, Data integration and Data augmentation
*	[DataPreparator](http://www.datapreparator.com/), Java based tool to explore, manipulate, transform and prepare data using a graphical user interface.
*	[Datamartist](http://www.datamartist.com/), allows large amounts of data from multiple sources to be combined together, enhanced and repaired without the need for database development.
*	[Datatect](http://datatect.software.informer.com/), a powerful program for generating realistic test data to ASCII flat files or directly to RDBMS including Oracle, Sybase, SQL Server, and Informix.
*	[DQ Now](http://www.dqnow.com/), profiling, cleansing, and dedup tools, providing a clear view of the data
*	[DQ Global](https://www.dqglobal.com/), data cleansing, data management software, including de-duplication, merge/purge, address correction and suppression.
*	[GritBot](https://www.rulequest.com/gritbot-info.html), for identifying anomalies in data (compatible with See5 and Cubist).
*	[Hummingbird ET](http://www.ewsolutions.com/resource-center/rwds_folder/rwds-archives/rwds-2003-07/genio-new-name)L, powerful data integration solution.
*	[MiningMart](http://mmart.cs.uni-dortmund.de/) platform, for the preparation of relational data for Knowledge Discovery, free for research and non-commercial applications.
*	[MoData](http://www.mo-data.com/) technology platform aggregates, cleanses and generates analytic cubes from disparate ERP and CRP sources and provides a data science and insights delivery platform.
*	[Sagent](http://www.pitneybowes.com/us/customer-information-management/data-integration-management/sagent-data-flow.html), provides a suite of data transformation and loading tools
*	[The Software Bureau](https://www.thesoftwarebureau.com/), providing Cygnus and SwiftSort innovative data quality software.
*	[Syncsort](http://www.syncsort.com/fr/Products), fast high-volume sorting, filtering, reformatting, aggregating, and more
*	[The TrueData COMponent](https://www.componentsource.com/product/componentone-studio-enterprise/reviews/2188678), functions to programmatically standardise your data, process it phonetically, and output a match key.
*	[Drake](https://github.com/Factual/drake), Drake is a simple-to-use, extensible, text-based data workflow tool that organizes command execution around data and its dependencies. Data processing steps are defined along with their inputs and outputs and Drake automatically resolves their dependencies and calculates: which commands to execute (based on file timestamps) in what order to execute the commands (based on dependencies). Drake is similar to GNU Make, but designed especially for data workflow management. It has HDFS support, allows multiple inputs and outputs, and includes a host of features designed to help you bring sanity to your otherwise chaotic data processing workflows.
*	[DataCleaner](https://datacleaner.org/), The heart of DataCleaner is a strong data profiling engine for discovering and analyzing the quality of your data. Find the patterns, missing values, character sets and other characteristics of your data values. Profiling is an essential activity of any Data Quality, Master Data Management or Data Governance program. If you don't know what you're up against, you have poor chances of fixing it.
*	[WinPure](http://www.winpure.com/) Data Cleaning Tool, Data quality is an important contributor in the overall success of a project or campaign. Inaccurate data leads to wrong assumptions and analysis. Consequently it leads to failure of the project or campaign. Duplicate data can thus cause all sorts of hassles such as slow load ups, accidental deletion etc. A good data cleaning tool tackles these problems and cleans your database of duplicate data, bad entries and incorrect information.


## Data extraction from the web

Various types of data exist on the web (text, image, video, etc.). Some web sites propose direct links to download the data (e.g.
specialized data repositories, see section Open Data), other propose APIs to
access the data usually stored in proprietary databases (scientific
journals, etc.). In many cases where the data is accessible using APIs, a
registration and/or processing fees are required to get the data.

## Analyse textual data

Text mining is the set of technologies allowing analysing textual data
either using statistical methods or natural language processing.

Here is a list of open source text mining tools and toolkits for
programming languages \[1\].

-   [Gargantext](https://iscpif.fr/projects/gargantext/) : a web
    service that combines **advanced text-mining, network analysis and
    interactive visualisation** to provide new forms of interactions
    with the users’ corpora. (Registration required)

-   [Carrot2](http://project.carrot2.org//) : text and search
    results clustering framework.

-   [GATE](https://gate.ac.uk/)
    : General Architecture for Text Engineering, an open-source toolbox
    for natural language processing and language engineering.

-   [Gensim](https://pypi.python.org/pypi/gensim) : large-scale topic
    modelling and extraction of semantic information from unstructured
    text ([Python](https://www.python.org)).

-   [OpenNLP](https://opennlp.apache.org/) : natural
    language processing.

-   [Orange](http://orange-text.readthedocs.io/en/latest/) :
    with a text mining add-on.

-   [Stanbol](https://en.wikipedia.org/wiki/Apache_Stanbol) : An open
    source text mining engine targeted at semantic content management.

-   The [KNIME Analytics Platform](http://www.knime.org/knime-analytics-platform) :
    a powerful tool for analysing datasets with a text processing extension : Text Processing.

-   [Natural Language Toolkit](http://www.nltk.org/)
    (NLTK) : a suite of libraries and programs for symbolic and
    statistical natural language processing (NLP) for the
    [Python](https://www.python.org) programming language.

-   The programming language [R](https://cran.r-project.org) :
    provides a framework for text mining applications in the package
    *tm*. The Natural Language Processing task view contains *tm* and
    other text mining library packages.

### Learn more..
If you need to know more about **free corpora** and **text mining tools** , you can visit this [link](http://libguides.usc.edu/textmining/tools).

## Use of semantic technologies to annotate and search data

In order to query the large content stored on the web or in large
document repositories, search engines are used such as Google, Yahoo,
etc. In many cases, queries are complex (natural language queries,
relational queries, multiple-words queries, etc.) and users do not
manage to find the information they are looking for.

Classic information retrieval techniques for content description and
query processing are based on keywords: documents are considered as
bag-of-words, only words existing in the document can be used to
retrieve them. The content meanings and the conceptualisation of the
user’s query are not exploited: (“jaguar” as animal or as car, “movie”
synonym of “film”, “cat” is a mammal, etc.).

Semantic information retrieval aims at solving this problem by using
content meanings to retrieve documents rather than single keywords.
Semantic technologies (RDFa, OWL ontologies) are used to semantically
annotate documents and understand users queries. RDFa adds semantic
information to HTML documents.  Ontologies consist on a set of
**classes + instances + semantic relations + rules** that help enriching documents
content. Based on these technologies, semantic search systems are able
to consider various points including context of search, location,
intent, variation of words, synonyms, generalized and
specialized queries, concept matching and natural
language queries to provide relevant search results \[2\].

**Example**:

Let’s consider an example of a simple user query “*rural road
île-de-france*”. In a classic IR system only documents containing these
terms are returned. With a semantic IR system, a semantic expansion of
the query leads to return documents containing for example:
*countryside* or *agricultural* as they are synomyms of the term
*rural*.

### Learn more..

Here after some usefull links to learn more about semantic annotation and search :
-   From Ontotext web site : [semantic annotation](ontotext.com/knowledgehub/fundamentals/semantic-annotation/)
-   Uren, Victoria; Cimiano, Philipp; Iria, Jose; Hanndschuh, Siegfried; Vargas-Vera, Maria; Motta, Enrico and Ciravegna, Fabio (2006). *Semantic annotation for knowledge management: requirements and a survey of the state of the art*. Journal of Web Semantics: Science, Services and Agents on the World Wide Web, 4(1) pp. 14–28.


### References

\[1\]
[*https://en.wikipedia.org/wiki/List\_of\_text\_mining\_software*](https://en.wikipedia.org/wiki/List_of_text_mining_software)

\[2\] John, Tony (January 2, 2017). [*"What is Semantic Search?"*](http://www.techulator.com/resources/5933-What-Semantic-Search.aspx).
