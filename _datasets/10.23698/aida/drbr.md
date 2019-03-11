---
title: "10.23698/aida/drbr"
datacite:
  "@context": "http://schema.org"
  "@type": "Dataset"
  "@id": "https://doi.org/10.23698/aida/drbr"
  name: "Breast data from the Visual Sweden project DROID"
  publicationYear: 2019
  about: "Pathology"
  url: "https://doi.aida.medtech4health.se/10.23698/aida/drbr"
  author:
    - "@type": "Person"
      "@id": "https://orcid.org/0000-0002-0128-870X"
      givenName: "Anna"
      familyName: "Bodén"
      name: "Anna Bodén"
    - "@type": "Person"
      "@id": "https://orcid.org/" # FIXME: missing info
      givenName: "Jerónimo"
      familyName: "Rose"
      name: "Jerónimo F. Rose"
    - "@type": "Person"
      "@id": "https://orcid.org/" # FIXME: missing info
      givenName: "Martin"
      familyName: "Lindvall"
      name: "Martin Lindvall"
    - "@type": "Person"
      "@id": "https://orcid.org/0000-0001-7250-234X"
      givenName: "Caroline"
      familyName: "Bivik Stadler"
      name: "Caroline Bivik Stadler"
  publisher:
    "@type": "Organization"
    name: "AIDA"
  copyrightYear: 2019
  copyrightHolder:
    - "@type": "Organization"
      name: "Linköping University"
      url: "https://liu.se/"
    - "@type": "Person"
      "@id": "https://orcid.org/0000-0002-9368-0177"
      givenName: "Claes"
      familyName: "Lundström"
      name: "Claes Lundström"
  provider:
    - "@type": "Person"
      "@id": "https://orcid.org/0000-0002-0128-870X"
      name: "Anna Bodén"
      email: "Anna.C.Boden@regionostergotland.se"
    - "@type": "Person"
      "@id": "https://orcid.org/0000-0002-9368-0177"
      name: "Claes Lundstrom"
      email: "claes.lundstrom@liu.se"
    - "@type": "Person"
      "@id": "https://orcid.org/0000-0001-6443-3604"
      name: "Joel Hedlund"
      email: "joel.hedlund@liu.se"
  dateCreated: "2019-01-09"
  datePublished: "2019-01-09"
  dateModified: "2019-01-09"
  keywords: "pathology, whole slide imaging, annotated"
  version: "1.0"
  description: |
    This dataset consists of 337 whole slide images (WSI) - 272 malignant from
    women with invasive breast cancer (HER2 neg) and 65 benign. The tumours have
    been classified with four SNOMED-CT categories based on morphology: invasive
    duct carcinoma, invasive lobular carcinoma, in situ carcinoma, and others.
    4381 separate annotations have been made to segment different tissue
    structures connected to ontologies.
  rightsList:
    - rights: "Restricted access"
      rightsURI: "#license"
  citation:
    - "@type": "CreativeWork" # FIXME: Incorrect entry for testing.
      "@id": "https://doi.org/10.5438/0000-00SS"
      name: "Title of paper 1 goes here"
    - "@type": "CreativeWork" # FIXME: Incorrect entry for testing.
      "@id": "http://dublincore.org/documents/2012/06/14/dces"
      name: "Title of paper 2 goes here"
    - "@type": "CreativeWork" # FIXME: Incorrect entry for testing.
      "@id": "https://doi.org/10.5438/TNHX-54CG"
      name: "Title of paper 3 goes here"
other:
  status: "Completed"
  annotation: |
    The breast tumours were classified with four SNOMED-CT categories based on
    morphology: invasive duct carcinoma, Invasive lobular carcinoma, in situ
    carcinoma and others. 4381 separate annotations were made to segment
    different tissue structures connected to ontologies. One physician were
    responsible for the manual annotations controlled by a second pathologist.
  ethicsApproval: |
    The data collection and sharing is ethical approved.
  license: "#license"
  download:
    links:
      - text: ""
        url: ""
  organ:
    - name: "Breast"
      "@id": "http://purl.org/sig/ont/fma/fma9601" # <- FIXME: this url doesn't work. What's a good ontology to use anyway?
  age-span: "-"
  bytes: 25000000000 # FIXME: is this correct?
  numberOfImages: 337
  numberOfAnnotations: 4381
  resolution: "40X single plane, scanned in NDP format"
  modality:
    - "Hamamatsu NanoZoomer-XR C12000 series 2013"
    - "Hamamatsu NanoZoomer 2.0 HT C9600 series 2013"
  stain: "H&E (hematoxylin and eosin)"
  phase:
  exampleImage:
    - title: "A random free-to-reuse breast pathology picture I found somewhere."
      url: "/assets/images/10.23698/aida/drbr/unrelated-picture.jpg"      
      thumbnail-url: "/assets/images/10.23698/aida/drbr/unrelated-picture-thumbnail.jpg"      
    - title: "A random free-to-reuse breast pathology picture I found somewhere."
      url: "/assets/images/10.23698/aida/drbr/unrelated-picture.jpg"
      thumbnail-url: "/assets/images/10.23698/aida/drbr/unrelated-picture-thumbnail.jpg"      
    - title: "A random free-to-reuse breast pathology picture I found somewhere."
      url: "/assets/images/10.23698/aida/drbr/unrelated-picture.jpg"
      thumbnail-url: "/assets/images/10.23698/aida/drbr/unrelated-picture-thumbnail.jpg"      
---
## License
Copyright {{ page.datacite.copyrightYear }} {{ page.datacite.copyrightHolder | map: "name" |  join: ", " }}

Permission to use, copy, modify, and/or distribute this data within Analytic
Imaging Diagnostics Arena ([AIDA](https://medtech4health.se/aida)) for any
purpose with or without fee is hereby granted, provided that the above copyright
notice and this permission notice appear in all copies, and that publications
resulting from the use of this data cite the following works:

{{ page.datacite.author | map: "name" | array_to_sentence_string }} ({{ page.datacite.publicationYear }}) {{ page.datacite.name }} [{{ page.datacite['@id'] | remove: "https://doi.org/" }}]({{ page.datacite["@id"] }}).

THE DATA IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD
TO THIS DATA INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN
NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR
CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA
OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR CHARACTERISTICS OF THIS
DATA.
