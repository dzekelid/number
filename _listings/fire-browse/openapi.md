---
swagger: "2.0"
x-collection-name: Fire Browse
x-complete: 1
info:
  title: Fire Browse Beta API
  description: a-simple-and-elegant-way-to-explore-cancer-data
  version: 1.1.35 (2016-09-27 10:12:23 6a47e74011281b2aa
host: firebrowse.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Analyses/CopyNumber/Genes/All:
    get:
      summary: Retrieve all data by genes Gistic2 results.
      description: 'This service provides access to the Gistic2 all_data_by_genes.txt
        output data. This data is a gene-level table of copy number values for all
        samples. The returned copy number values are in units (copy number - 2) so
        that no amplification or deletion is 0, genes with amplifications have positive
        values, and genes with deletions are negative values. The data are converted
        from marker level to gene level using the extreme method: a gene is assigned
        the greatest amplification or the least deletion value among the markers it
        covers. Results may be filtered by cohort, gene, or barcode, but at least
        one gene or barcode must be supplied.'
      operationId: getAnalysesCopynumberGenesAll
      x-api-path-slug: analysescopynumbergenesall-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      - in: query
        name: gene
        description: Comma separated list of gene name(s)
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      - in: query
        name: tcga_participant_barcode
        description: Comma separated list of TCGA participant barcodes (e
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - CopyNumber
      - Genes
  /Analyses/CopyNumber/Genes/Amplified:
    get:
      summary: Retrieve Gistic2 significantly amplified genes results.
      description: This service provides access to the Gistic2 amp_genes.conf_99.txt
        output data.  At least 1 gene or cohort must be supplied.
      operationId: getAnalysesCopynumberGenesAmplified
      x-api-path-slug: analysescopynumbergenesamplified-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      - in: query
        name: gene
        description: Comma separated list of gene name(s)
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: q
        description: Only return results with Q-value
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - CopyNumber
      - Genes
      - Amplified
  /Analyses/CopyNumber/Genes/Deleted:
    get:
      summary: Retrieve Gistic2 significantly deleted genes results.
      description: This service provides access to the Gistic2 del_genes.conf_99.txt
        output data.  At least 1 gene or cohort must be supplied.
      operationId: getAnalysesCopynumberGenesDeleted
      x-api-path-slug: analysescopynumbergenesdeleted-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      - in: query
        name: gene
        description: Comma separated list of gene name(s)
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: q
        description: Only return results with Q-value
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - CopyNumber
      - Genes
      - D
  /Analyses/CopyNumber/Genes/Focal:
    get:
      summary: Retrieve focal data by genes Gistic2 results.
      description: 'This service provides access to the Gistic2 focal_data_by_genes.txt
        output data. This output is similar to the all_data_by_genes.txt output, but
        using only focal events with lengths greater than the  focal length cutoff.
        This data is a gene-level table of copy number values for all samples. The
        returned copy number values are in units (copy number - 2) so that no amplification
        or deletion is 0, genes with amplifications have positive values, and genes
        with deletions are negative values. The data are converted from marker level
        to gene level using the extreme method: a gene is assigned the greatest amplification
        or the least deletion value among the markers it covers. Results may be filtered
        by cohort, gene, and/or barcode, but at least one gene or barcode must be
        supplied.'
      operationId: getAnalysesCopynumberGenesFocal
      x-api-path-slug: analysescopynumbergenesfocal-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      - in: query
        name: gene
        description: Comma separated list of gene name(s)
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      - in: query
        name: tcga_participant_barcode
        description: Comma separated list of TCGA participant barcodes (e
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - CopyNumber
      - Genes
      - Focal
  /Analyses/CopyNumber/Genes/Thresholded:
    get:
      summary: Retrieve all thresholded by genes Gistic2 results.
      description: 'This service provides access to the Gistic2 all_thresholded_by_genes.txt
        output data. A gene-level table of discrete amplification and deletion indicators
        for all samples. A table value of 0 means no amplification or deletion above
        the threshold. Amplifications are positive numbers: 1 means amplification
        above the amplification threshold; 2 means amplifications larger to the arm
        level amplifications observed for the sample. Deletions are represented by
        negative table values: -1 represents deletion beyond the threshold; -2 means
        deletions greater than the minimum arm-level deletion observed for the sample.
        Results maybe filtered by cohort, gene or barcode, but at least one gene or
        barcode must be supplied.'
      operationId: getAnalysesCopynumberGenesThresholded
      x-api-path-slug: analysescopynumbergenesthresholded-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      - in: query
        name: gene
        description: Comma separated list of gene name(s)
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      - in: query
        name: tcga_participant_barcode
        description: Comma separated list of TCGA participant barcodes (e
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - CopyNumber
      - Genes
      - Thresholded
---