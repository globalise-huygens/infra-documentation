We draw on various **external sources** of data to prepare curated LOD datasets of e.g. commodities, ships, and polities along with their taxonomies and ontologies.  ^f3878b

The external sources are varied, and range from entirely unstructured material such as printed texts, to already digitised and (semi-)structured (but not yet LOD qualified) datasets. Two examples are the [Boekhouder Generaal Batavia (BGB)](https://resources.huygens.knaw.nl/boekhoudergeneraalbatavia) database for commodities and the [Dutch Asiatic Shipping](https://resources.huygens.knaw.nl/das/) database. Both are hosted at the Huygens Institute. In order to properly structure these lists, and make them LOD compatible, we prepare taxonomies and vocabularies in [PoolParty](https://digitaalerfgoed.poolparty.biz/globalise.html) to define the concepts we use to describe, for example, what types of cloth (cotton, linen, silk..) was traded by the VOC.  

Items such as lists of ships and commodities are currently curated in Excel/Google Sheets (later in Django). Concepts (such as thesauri and ontologies) are curated and hosted in [[Concepts (PoolParty)|PoolParty]]. 

### status:

- in use

### pipeline:

- Input: Typically CSV files obtained manually from diverse sources
- Transformation: [[Curation (Spreadsheets)|Curated]] manually in Excel/Google Sheets and [[Metadata Curation (Django)|Django]] (items); or [[Concepts (PoolParty)|PoolParty]] (concepts). Conversion into RDF (manually for items, automatically for concepts) 
- Output: RDF to [[Knowledge Graph (GraphDB)]]

### hosted:

- Excel/Google Sheets (manual backups to SurfDrive)
- PoolParty: [hosted at RCE](https://digitaalerfgoed.poolparty.biz/globalise.html ) (manual backups to SurfDrive)
- Django: VM on Globalise dev. server (DI-CI backups)

### owners:

- Leon: import/export, data conversions and transformation
- Manjusha: WP3 lead for curation 
- Vic: Django development

### future plans:

- Move the majority of Excel/Google curation work to Django so that records can be properly interlinked

### references:

- [Blogpost on curation process](https://globalise.huygens.knaw.nl/rediscovering-early-modern-polities-first-thoughts-on-dataset-creation/)
- [Units of Measure - Dataset and Documentation](https://github.com/globalise-huygens/globalise-units-of-measure)
- [Persons Dataset - Dataset and Documentation](https://github.com/globalise-huygens/personsdataset)
- [Commodities Dataset early versions in Excel and Documentation](https://github.com/globalise-huygens/globalise-vocabulary)
- [South Asia Glossary: Dataset in Excel and Documentation](https://github.com/globalise-huygens/globalise-south-asia-glossary)
- [Locations Dataset in Excel and Documentation](https://github.com/globalise-huygens/globalise-places)
- [Polities Dataset in Excel and Documentation](https://drive.google.com/drive/folders/1qK3SqYnfDJMGbKHQtlt9FJhO8A351PGj)
- [Surfdrive: Sources for all datasets, incl. early versions of locations and places, backup for polities dataset, most WP3 work from 2022](https://surfdrive.surf.nl/files/index.php/apps/files/?dir=/Shared/GLOBALISE_shared_team/wp3&fileid=11788542838)
- [Thesaurus for Globalise Concepts and Categories](https://digitaalerfgoed.poolparty.biz/PoolParty/)
