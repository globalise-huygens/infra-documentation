





TextRepo

`Inside the TR, conversion of PageXML into documents (start and end files)
`Sophie needs to get in TBD format, text via the API (which will would provide the requested serialization), to pre-annotate. Currently, from Sophie, directly to Inception, likely in WebAnno-TSV v3.x. 

Inception

`Three separate tasks in Inception. Entity annotation, X is Person, then disambiguate X through entity linking, drawing on the reference data in Graph DB (Inception generates a SPARQL query against the GraphDB), events annotation, the ontology to whitich all annotations must conform was pre-imported by hand in Inception. Stella wants to also disambiguate events, event co-reference resolution. How can you link two events in two documents (Inception doesn't let you refer to the same event in another document). PoolParty manages concepts, made available together with invididual instances of e.g. people, in the KG, in GraophDB, which in turn is what Inception queries. 

`We need to decide when annotations are ready to be passed on to the AnnoRepo. At point of annotation? After explicit save? After further curation? TBD. 

`At present manual export from Inception for AnnoRepo, WebAnno TSV, most likely the export format. Bram converts this into WebAnnotations (as required by AnnoRepo). Might in the future query the Inception API for this purpose. 

To build the NER and event model, the current thinking is to get annotations (in WebAnno TSV) and underlying via Broccoli, which in turn will query the Annorepo and Textrepo for this. TBD
Also TBD where and how the model would run, etc. In effect, parallel to how Sphie sends pre-annotated text to Inception (though now it would go to the AnnoRepo). Brocolli can give everything  provided via collection metadat plus our enrichment (e.g. parapgraphs, sigs, document boundaries).  One web application that can take advantage is textannoviz. 


Copy AnnoRepo annotations to Graph via RDF, not done yet. ElasticSearch is an endpoint of the TextRepo. 



