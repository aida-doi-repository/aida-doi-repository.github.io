---
title: "10.23698/aida/drske"
image: "/assets/images/10.23698/aida/drske/unrelated-picture.jpg"
seo:
  description: "Skeletal data from the Visual Sweden project DROID"
  image: "/assets/images/10.23698/aida/drske/unrelated-picture.jpg"
datacite:
  "@context": "http://schema.org"
  "@type": "Dataset"
  "@id": "https://doi.org/10.23698/aida/drske"
  image: "/assets/images/10.23698/aida/drske/unrelated-picture.jpg"
  name: "Skeletal data from the Visual Sweden project DROID"
  publicationYear: 2019
  about: "Radiology"
  url: "https://doi.aida.medtech4health.se/10.23698/aida/drske"
  author:
    - "@type": "Person"
      "@id": "https://orcid.org/0000-0003-0066-4985"
      givenName: "Mischa"
      familyName: "Woisetschläger"
      name: "Mischa Woisetschläger"
    - "@type": "Person"
      "@id": "https://orcid.org/" # FIXME: missing info
      givenName: "Filip"
      familyName: "Landgren"
      name: "Filip Landgren"
    - "@type": "Person"
      "@id": "https://orcid.org/0000-0001-7250-234X"
      givenName: "Caroline"
      familyName: "Bivik Stadler"
      name: "Caroline Bivik Stadler"
    - "@type": "Person"
      "@id": "https://orcid.org/0000-0003-0908-9470	"
      givenName: "Daniel"
      familyName: "Forsberg"
      name: "Daniel Forsberg"
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
      "@id": "https://orcid.org/0000-0003-0066-4985"
      name: "Mischa Woisetschläger"
      email: "Mischa.Woisetschlager@regionostergotland.se"
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
  keywords: "bone metastasis, radiology, annotated"
  version: "1.0"
  description: |
    36 radiology cases showing lytic and lytic/sclerotic (blastic) metastases
    i.e. bone regenerative and degenerative. These cases have all been punctured
    and pathologically analyzed to verify the diagnose. The metastases were
    segmented accurately by a radiologist and the annotations were confirmed by
    a second radiologist.
  rightsList:
    - rights: "Restricted access"
      rightsURI: "#license"
  citation:
    - "@type": "CreativeWork"
      "@id": "https://doi.org/10.5438/0000-00SS"
      name: "Title of paper 1 goes here"
    - "@type": "CreativeWork"
      "@id": "http://dublincore.org/documents/2012/06/14/dces"
      name: "Title of paper 2 goes here"
    - "@type": "CreativeWork"
      "@id": "https://doi.org/10.5438/TNHX-54CG"
      name: "Title of paper 3 goes here"
    - "@type": "CreativeWork"
      "@id": "https://doi.org/10.5438/55E5-T5C0"
      name: "Title of paper 4 goes here"
    - "@type": "CreativeWork"
      "@id": "https://doi.org/10.5438/4K3M-NYVG"
      name: "Title of paper 5 goes here"
other:
  status: "Completed"
  annotation: |
    The metastases were segmented accurately by a radiologist and the
    annotations were confirmed by a second radiologist.
  ethicsApproval: |
    The data collection and sharing is ethical approved.
  license: "#license"
  download:
    links:
      - text: ""
        url: ""
  organ:
    - name: "Bone" # FIXME: Is this correct? What's a good ontology to use anyway?
      "@id": "" # FIXME: Missing data.
  age-span: "-"
  bytes: 25000000000 # FIXME: is this correct?
  numberOfImages: 36
  numberOfAnnotations:
  resolution:
  modality:
  stain:
  phase:
  exampleImage:
    - title: "A random free-to-reuse ct chest picture I found somewhere."
      url: "/assets/images/10.23698/aida/drske/unrelated-picture.jpg"
      thumbnail-url: "/assets/images/10.23698/aida/drske/unrelated-picture-thumbnail.jpg"
    - title: "A random free-to-reuse ct chest picture I found somewhere."
      url: "/assets/images/10.23698/aida/drske/unrelated-picture.jpg"
      thumbnail-url: "/assets/images/10.23698/aida/drske/unrelated-picture-thumbnail.jpg"
    - title: "A random free-to-reuse ct chest picture I found somewhere."
      url: "/assets/images/10.23698/aida/drske/unrelated-picture.jpg"
      thumbnail-url: "/assets/images/10.23698/aida/drske/unrelated-picture-thumbnail.jpg"
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
