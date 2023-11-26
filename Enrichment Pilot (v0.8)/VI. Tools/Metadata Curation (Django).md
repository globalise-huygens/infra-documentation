We are using the Python Django framework and admin tool to create web apps for curating **structured reference data**. ^2d8988

Django uses Postgres as its data store with a data model defined in code in the Django app. 

### status:

- in use & development

### pipeline:

- Input: Manually as CSV, add/delete/edit via web interface
- Transformation: curation and contextualisation 
- Output: At present, manual export as CSV > python conversion script to RDF > [Knowledge Graph](Knowledge%20Graph%20(GraphDB).md). 

### hosted:

- CI in Kubernetes (DI-CI backups)

### owners:

- Leon: data models w/Vic & Manjusha, conversions
- Manjusha: Overall lead for curation
- Vic: Django development

### future plans:

- (Automatic) annotations will identify new entities and types of entities not anticipated / present in our structured reference data - how do we deal with these?

### references:

- 
