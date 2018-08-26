{
  "info": {
    "name": "Fire Browse Beta API Retrieve Gistic2 significantly amplified genes results.",
    "_postman_id": "3ac21277-20af-4f1e-b020-a2057ddd99d1",
    "description": "This service provides access to the Gistic2 amp_genes.conf_99.txt output data.  At least 1 gene or cohort must be supplied.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Analyses",
      "item": [
        {
          "id": "f0ecc98d-8cb3-4996-a93c-949fefa0f2c9",
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
              "id": "1c3344aa-91f9-49ea-a957-f3d9d98be17b"
            }
          ]
        },
        {
          "id": "149c4ca2-47e6-4992-9e7e-ae579981fd6b",
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
              "id": "7a751f4a-5ffe-4deb-a761-0bb22d5c535d"
            }
          ]
        }
      ]
    }
  ]
}