**HTR conversion** of page images to PageXML transcripts including labelled layout elements in basic reader order. ^ac2720

### status:

- in use

### pipelines:

- Input: JPEG page images from [National Archives](National%20Archives.md) (c. 22TB)
- Transformation: pre-processing, HTR, post-processing
- Output: PageXML and metadata to [PIM](Transcriptions%20(PIM).md) and [TextRepo](Transcriptions%20(TextRepo).md)

### hosted:

- HTR: GPU-server
- Transcripts: [PIM](Transcriptions%20(PIM).md) and [TextRepo](Transcriptions%20(TextRepo).md)
- Offline backups: USB HDDs in Globalise office (also of first, in part lower quality version of the images used for the initial, March 2023 output)

### owners:

- Rutger: HTR on Loghi, PIM
- Lodewijk: Overall lead for HTR
- Hennie: Overall lead for TextRepo

### future plans:  

- Optimize post HTR workflow (e.g. improved region detection, language identification)

### references:

- https://globalise.huygens.knaw.nl/the-ground-truth-is-out-there-an-introduction-to-globalises-use-of-handwritten-text-recognition/ (blogpost)
