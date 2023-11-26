The **National Archives** are our source for the JPEG images, EAD and METS files for the VOC corpus.  ^61dac5

Since the NA does not make its highest quality JPEG files available via a public IIIF endpoint, and (based on past experience) downloading these would take several months, we arranged for the files to be provided to us by the NA on external HDDs (via a private IIIF endpoint only accessible from the NA e-depot). The images are then transferred onto the GPU-server directly from the HDDs. 

### status:

- in use

### pipeline:

- Input: n/a
- Transformation: n/a
- Output: JPEG images to [[HTR (Loghi)|GPU server]] (manual process)
- Output: EAD and METS XML files to [[Transcriptions (TextRepo)|TextRepo]] (manual process)

### hosted:

- National Archives (IIIF endpoints for images, public website for EADs and APIs for METS)

### owners:

- Rutger: Obtain JPEGs from NA and transfer to GPU-server
- Leon: Copy EADs and METS from NA website and give to team text
- Lodewijk: Overall lead for HTR

### future plans:  

- Convert the EAD files to a LOD compatible RDF format using the Records in Context ontology (EAD RIC-O) and make them available in the Knowledge Graph via SPARQL endpoint. Our hope is that (part of) this is done by the NA, but we are prepared to do this ourselves if necessary.
- In the future, as part of the work for OvR, the NA will provide metadata on the collection in web annotation format via the IIIF manifest

### references:

+ https://www.nationaalarchief.nl/onderzoeken/archief/1.04.02 (Source files)

