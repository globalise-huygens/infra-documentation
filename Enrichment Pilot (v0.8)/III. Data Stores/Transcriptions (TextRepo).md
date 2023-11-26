Data store for **PageXML transcriptions** organised (where possible) as documents, their variants, related metadata and annotation references.  ^872d59

In the TextRepo, metadata from the NA's EAD files are used to fix a document's start and end files. Texts and associated metadata are stored in PostgreSQL. Search index in ElasticSearch.

### status:

- in use

### pipelines:

- Input: Manual import of PageXMLs plus metadata (e.g. document extents), currently from [[Project Data (HuCDrive)]]
- Transformations: n/a
- Output: Relevant text elements (in appropriate serialisation) via TextRepo API

### hosted:

- Kubernetes (DI-CI backups)

### owners:

- Hennie: Overall lead for TextRepo

### future plans:  

- 

### references:

- https://github.com/knaw-huc/textrepo (Source code on GitHub)
- https://textrepo.readthedocs.io/en/stable/ (Technical documentation)