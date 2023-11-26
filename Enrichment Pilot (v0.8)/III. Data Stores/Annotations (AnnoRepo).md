All **annotated enrichments** to the transcripts, including all variants and versions, stored as web annotations. ^5016ec

A webservice for W3C Web Annotations, implementing the W3C Web Annotation Protocol, plus custom services (batch upload, search, etc.). The annotations are stored and queried in MongoDB.

### status:

- in use, and in further development

### pipelines:

- Input: Manual import as Web Annotation TSV from [Annotation Editor (Inception)](Annotation%20Editor%20(Inception).md)
- Transformation: Conversion to WebAnno format, later possibly via Inception API
- Output: multiple (e.g. drawn on by [HTR Viewer (TextAnnoViz)](HTR%20Viewer%20(TextAnnoViz).md) via [Intermediary Service (Broccoli)](Intermediary%20Service%20(Broccoli).md) to render annotations)

### hosted:

- VM (DI-CI backups), later Kubernetes
- PostgreSQL (data), ElasticSearch (index); DI-CI backups

### owners:

- Hennie: Overall lead for AnnoRepo

### future plans:  

- tba

### references:

- https://github.com/knaw-huc/annorepo (Source code on GitHub)
- https://knaw-huc.github.io/annorepo/docs/usage.html (Technical documentation)