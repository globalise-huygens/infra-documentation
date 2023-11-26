Custom **NLP pipelines** to detect and disambiguate selected **entities** (e.g. polities, persons, and commodities). ^c0c297

### status:

- in development, initial test results available (Nov. 2023)

### pipelines:

- Input: UIMA CAS XMI via [TextRepo](Transcriptions%20(TextRepo).md) API
- Transformation: recognize entities (type and entity reference), record character ranges
- Output: UIMA CAS XMI to [AnnoRepo](Annotations%20(AnnoRepo).md)

### hosted:

- tbd - models to run on the GPU server (ant)

### owners:

- Sophie: Overall lead for NER

### future plans:  

- Revise model drawing on data from January 2024 annotation spring

### references:

- https://github.com/cltl/voc-missives/ (code and data for Named Entity Recognition (NER) on the edition of the [VOC's General Letters](https://resources.huygens.knaw.nl/vocgeneralemissiven) hosted at the Huygens Institute. This project was part of Clariah WP6/Text).
- https://github.com/globalise-huygens/nlp-pilot-code: pilot code for NER enrichment through string matching and pretrained model (based on the Clariah work) 
