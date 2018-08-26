{
  "info": {
    "name": "Fire Browse Beta API Retrieve Gistic2 significantly deleted genes results.",
    "_postman_id": "50956487-9df6-47ce-8b4c-3600b21e689f",
    "description": "This service provides access to the Gistic2 del_genes.conf_99.txt output data.  At least 1 gene or cohort must be supplied.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Analyses",
      "item": [
        {
          "id": "1e5ee761-6bc1-4807-919c-ce0194036152",
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
              "id": "620344ad-95a0-4a5c-b085-c08546b8b631"
            }
          ]
        },
        {
          "id": "3cbc8d8e-5909-48d5-8b2b-db4c9d6c4b6c",
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
              "id": "82d56724-78bd-42f9-bc1a-725817d4edd5"
            }
          ]
        },
        {
          "id": "88f2d809-c3c1-4a87-b6c5-f1e63e5255a2",
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
              "id": "10e5fc5a-68c3-4643-a9a8-9517d0f6f114"
            }
          ]
        }
      ]
    }
  ]
}