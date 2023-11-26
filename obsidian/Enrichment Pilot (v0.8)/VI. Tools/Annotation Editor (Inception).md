**Inception** is used to create training data for entity and event detection.  ^6b2698

Reference data for entity linking is drawn from GraphDB to which all annotations must conform. Pool

### pipelines:

- Input: Manually, WebAnno TSV format
- Transformations: Annotations
- Output: Manual export to TextRepo in WebAnno TSV format

### hosted:

- DI-CI (Docker) at https://text-annotation.huc.knaw.nl

### owners:

- Lodewijk (application)
- Jordy (hosting, backups)

### future plans:  

- We need to decide when annotations are ready to be passed on to the AnnoRepo. At point of annotation? After explicit save? After further curation? 
- At what point do we switch to using the Inception API for import/export?

### references:

- [Inception project page](https://inception-project.github.io) and [release notes](https://github.com/inception-project/inception/releases)