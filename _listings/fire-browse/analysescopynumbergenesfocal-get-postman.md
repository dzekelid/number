{
  "info": {
    "name": "Fire Browse Beta API Retrieve focal data by genes Gistic2 results.",
    "_postman_id": "5ba2223b-f364-48fc-ab81-82efac41fd42",
    "description": "This service provides access to the Gistic2 focal_data_by_genes.txt output data. This output is similar to the all_data_by_genes.txt output, but using only focal events with lengths greater than the  focal length cutoff. This data is a gene-level table of copy number values for all samples. The returned copy number values are in units (copy number - 2) so that no amplification or deletion is 0, genes with amplifications have positive values, and genes with deletions are negative values. The data are converted from marker level to gene level using the extreme method: a gene is assigned the greatest amplification or the least deletion value among the markers it covers. Results may be filtered by cohort, gene, and/or barcode, but at least one gene or barcode must be supplied.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Analyses",
      "item": [
        {
          "id": "034e021c-724e-4053-8fed-74cb4079d3f7",
          "name": "getAnalysesCopynumberGenesAll",
          "request": {
            "url": "http://firebrowse.org/api/v1/Analyses/CopyNumber/Genes/All?cohort=%7B%7D&format=%7B%7D&gene=%7B%7D&page=%7B%7D&page_size=%7B%7D&sort_by=%7B%7D&tcga_participant_barcode=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service provides access to the Gistic2 all_data_by_genes.txt output data. This data is a gene-level table of copy number values for all samples. The returned copy number values are in units (copy number - 2) so that no amplification or deletion is 0, genes with amplifications have positive values, and genes with deletions are negative values. The data are converted from marker level to gene level using the extreme method: a gene is assigned the greatest amplification or the least deletion value among the markers it covers. Results may be filtered by cohort, gene, or barcode, but at least one gene or barcode must be supplied."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5615aa87-d567-4cd2-a980-4004ff7f8b3b"
            }
          ]
        },
        {
          "id": "c51a3a8d-3c32-4bd9-af1b-cbce9d3f36a1",
          "name": "getAnalysesCopynumberGenesAmplified",
          "request": {
            "url": "http://firebrowse.org/api/v1/Analyses/CopyNumber/Genes/Amplified?cohort=%7B%7D&format=%7B%7D&gene=%7B%7D&page=%7B%7D&page_size=%7B%7D&q=%7B%7D&sort_by=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service provides access to the Gistic2 amp_genes.conf_99.txt output data.  At least 1 gene or cohort must be supplied."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1be615c6-ccb6-48a5-9c0e-5f4f015d2484"
            }
          ]
        },
        {
          "id": "b88ce350-4522-465e-be3b-c8e26faddb8a",
          "name": "getAnalysesCopynumberGenesDeleted",
          "request": {
            "url": "http://firebrowse.org/api/v1/Analyses/CopyNumber/Genes/Deleted?cohort=%7B%7D&format=%7B%7D&gene=%7B%7D&page=%7B%7D&page_size=%7B%7D&q=%7B%7D&sort_by=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service provides access to the Gistic2 del_genes.conf_99.txt output data.  At least 1 gene or cohort must be supplied."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39ad2bc3-7d6e-4cc5-8e3d-6ad180887425"
            }
          ]
        },
        {
          "id": "a54bd03a-59cf-47d2-925d-af10e36ec385",
          "name": "getAnalysesCopynumberGenesFocal",
          "request": {
            "url": "http://firebrowse.org/api/v1/Analyses/CopyNumber/Genes/Focal?cohort=%7B%7D&format=%7B%7D&gene=%7B%7D&page=%7B%7D&page_size=%7B%7D&sort_by=%7B%7D&tcga_participant_barcode=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service provides access to the Gistic2 focal_data_by_genes.txt output data. This output is similar to the all_data_by_genes.txt output, but using only focal events with lengths greater than the  focal length cutoff. This data is a gene-level table of copy number values for all samples. The returned copy number values are in units (copy number - 2) so that no amplification or deletion is 0, genes with amplifications have positive values, and genes with deletions are negative values. The data are converted from marker level to gene level using the extreme method: a gene is assigned the greatest amplification or the least deletion value among the markers it covers. Results may be filtered by cohort, gene, and/or barcode, but at least one gene or barcode must be supplied."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f8f2655-81b3-4163-9571-b88716a141e5"
            }
          ]
        }
      ]
    }
  ]
}