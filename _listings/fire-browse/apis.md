---
name: Fire Browse
x-slug: fire-browse
description: A simple and elegant way to explore cancer data. Sitting above one of
  the deepest and most integratively characterized open cancer datasets in the world.
  Backed by a powerful computational infrastructure, application programming interface
  (API), graphical tools and online reports. With over 80K sample aliquots from 11,000+
  cancer patients, spanning 38 unique disease cohorts.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Number
created: "2018-08-25"
modified: "2018-08-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/number/master/_listings/fire-browse/apis.md
specificationVersion: "0.14"
apis:
- name: Fire Browse Beta API - Retrieve all data by genes Gistic2 results.
  x-api-slug: analysescopynumbergenesall-get
  description: 'This service provides access to the Gistic2 all_data_by_genes.txt
    output data. This data is a gene-level table of copy number values for all samples.
    The returned copy number values are in units (copy number - 2) so that no amplification
    or deletion is 0, genes with amplifications have positive values, and genes with
    deletions are negative values. The data are converted from marker level to gene
    level using the extreme method: a gene is assigned the greatest amplification
    or the least deletion value among the markers it covers. Results may be filtered
    by cohort, gene, or barcode, but at least one gene or barcode must be supplied.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1
  tags: Cancer, API Provider, Data Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/number/master/_listings/fire-browse/analysescopynumbergenesall-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/number/master/_listings/fire-browse/analysescopynumbergenesall-get-openapi.md
- name: Fire Browse Beta API - Retrieve Gistic2 significantly amplified genes results.
  x-api-slug: analysescopynumbergenesamplified-get
  description: This service provides access to the Gistic2 amp_genes.conf_99.txt output
    data.  At least 1 gene or cohort must be supplied.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1
  tags: Cancer, API Provider, Data Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/number/master/_listings/fire-browse/analysescopynumbergenesamplified-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/number/master/_listings/fire-browse/analysescopynumbergenesamplified-get-openapi.md
- name: Fire Browse Beta API - Retrieve Gistic2 significantly deleted genes results.
  x-api-slug: analysescopynumbergenesdeleted-get
  description: This service provides access to the Gistic2 del_genes.conf_99.txt output
    data.  At least 1 gene or cohort must be supplied.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1
  tags: Cancer, API Provider, Data Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/number/master/_listings/fire-browse/analysescopynumbergenesdeleted-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/number/master/_listings/fire-browse/analysescopynumbergenesdeleted-get-openapi.md
- name: Fire Browse Beta API - Retrieve focal data by genes Gistic2 results.
  x-api-slug: analysescopynumbergenesfocal-get
  description: 'This service provides access to the Gistic2 focal_data_by_genes.txt
    output data. This output is similar to the all_data_by_genes.txt output, but using
    only focal events with lengths greater than the  focal length cutoff. This data
    is a gene-level table of copy number values for all samples. The returned copy
    number values are in units (copy number - 2) so that no amplification or deletion
    is 0, genes with amplifications have positive values, and genes with deletions
    are negative values. The data are converted from marker level to gene level using
    the extreme method: a gene is assigned the greatest amplification or the least
    deletion value among the markers it covers. Results may be filtered by cohort,
    gene, and/or barcode, but at least one gene or barcode must be supplied.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1
  tags: Cancer, API Provider, Data Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/number/master/_listings/fire-browse/analysescopynumbergenesfocal-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/number/master/_listings/fire-browse/analysescopynumbergenesfocal-get-openapi.md
- name: Fire Browse Beta API - Retrieve all thresholded by genes Gistic2 results.
  x-api-slug: analysescopynumbergenesthresholded-get
  description: 'This service provides access to the Gistic2 all_thresholded_by_genes.txt
    output data. A gene-level table of discrete amplification and deletion indicators
    for all samples. A table value of 0 means no amplification or deletion above the
    threshold. Amplifications are positive numbers: 1 means amplification above the
    amplification threshold; 2 means amplifications larger to the arm level amplifications
    observed for the sample. Deletions are represented by negative table values: -1
    represents deletion beyond the threshold; -2 means deletions greater than the
    minimum arm-level deletion observed for the sample. Results maybe filtered by
    cohort, gene or barcode, but at least one gene or barcode must be supplied.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebrowse.png
  humanURL: http://firebrowse.org
  baseURL: https://firebrowse.org//api/v1
  tags: Cancer, API Provider, Data Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/number/master/_listings/fire-browse/analysescopynumbergenesthresholded-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/number/master/_listings/fire-browse/analysescopynumbergenesthresholded-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://factual.api.gallery.streamdata.io
- type: x-api-stack
  url: http://fire.browse.stack.network
- type: x-website
  url: http://firebrowse.org
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---