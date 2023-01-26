﻿## Repository description
<p>This is the command line utility that generates Species Annotations REVIGO uses to process data and create Similarity Matrix. 
The utility is computationaly intensive and threaded (parallelized). Be careful when you specify number of cores your CPU has.</p>

## How to compile and run
You need to obtain the following files to generate REVIGO databases:

* EBI GOA database, ftp://ftp.ebi.ac.uk/pub/databases/GO/goa/UNIPROT/goa_uniprot_gcrp.gaf.gz (Needs to be uncompressed, be careful, uncompressed size exceeds 50GB)
* NCBI database, ftp://ftp.ncbi.nlm.nih.gov/pub/taxonomy/taxdump.tar.gz (Needs to be uncompressed)
* Gene Ontology database, http://purl.obolibrary.org/obo/go.obo and https://www.uniprot.org/docs/keywlist.txt in same directory

Each directory containing a database also contains link.txt file containing a link to a database. For example EBI GOA link.txt file will contain the following: ftp://ftp.ebi.ac.uk/pub/databases/GO/goa/UNIPROT/goa_uniprot_gcrp.gaf.gz

After that adjust the paths to the databases and you are ready to go.

## About REVIGO (REduce + VIsualize Gene Ontology) project
<p>Outcomes of high-throughput biological experiments are typically interpreted by statistical testing
for enriched gene functional categories defined by the Gene Ontology (GO). The resulting lists of GO terms 
may be large and highly redundant, and thus difficult to interpret.<p>
<p>REVIGO is a successful project to summarize long, unintelligible lists of Gene Ontology terms by finding a representative subset 
of the terms using a simple clustering algorithm that relies on semantic similarity measures.</p>
<p>For any further information about REVIGO project please see 
<a href="https://dx.doi.org/10.1371/journal.pone.0021800" target="_blank">published paper</a> and 
<a href="http://revigo.irb.hr/FAQ.aspx" target="_blank">Frequently Asked Questions page</a></p>
