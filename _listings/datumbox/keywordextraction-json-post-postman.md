{
  "info": {
    "name": "Datumbox Extracts the Keywords of the Document",
    "_postman_id": "e5a8109c-4901-408b-802a-a522ebb82829",
    "description": "The Keyword Extraction function enables you to extract from an arbitrary document all the keywords and word-combinations along with their occurrences in the text.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Adult Content",
      "item": [
        {
          "id": "65bbb271-cac7-4526-8daf-bc2a985d6884",
          "name": "AdultContentDetection",
          "request": {
            "url": "http://api.datumbox.com/1.0/AdultContentDetection.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Adult Content Detection function classifies the documents as adult or noadult based on their context. It can be used to detect whether a document contains content unsuitable for minors."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1cbdd038-925d-4d47-bc1a-a0f32b252079"
            }
          ]
        }
      ]
    },
    {
      "name": "Commercial",
      "item": [
        {
          "id": "705bc756-6cdb-44e1-8731-e3a0441b0686",
          "name": "CommercialDetection",
          "request": {
            "url": "http://api.datumbox.com/1.0/CommercialDetection.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Commercial Detection function labels the documents as commercial or non-commercial based on their keywords and expressions. It can be used to detect whether a website is commercial or not."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "77ee7137-7a23-4a81-b648-58b37e7e9e17"
            }
          ]
        }
      ]
    },
    {
      "name": "DocumentsSimilarity",
      "item": [
        {
          "id": "911825a5-f279-4545-b306-b66257977b44",
          "name": "DocumentSimilarity",
          "request": {
            "url": "http://api.datumbox.com/1.0/DocumentSimilarity.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "copy",
                  "value": "{}",
                  "disabled": false,
                  "description": "The second text"
                },
                {
                  "key": "original",
                  "value": "{}",
                  "disabled": false,
                  "description": "The first text"
                }
              ]
            },
            "description": "The Document Similarity function estimates the degree of similarity between two documents. It can be used to detect duplicate webpages or detect plagiarism."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5ebe8e2-f80c-4036-a70c-53df3f32c9e5"
            }
          ]
        }
      ]
    },
    {
      "name": "Educational",
      "item": [
        {
          "id": "72bee4ca-26d5-47cc-b879-938680c9e354",
          "name": "EducationalDetection",
          "request": {
            "url": "http://api.datumbox.com/1.0/EducationalDetection.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Educational Detection function classifies the documents as educational or non-educational based on their context. It can be used to detect whether a website is educational or not."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c20c77e9-fe24-4a17-b36f-5bd4292ac50f"
            }
          ]
        }
      ]
    },
    {
      "name": "Gender",
      "item": [
        {
          "id": "1476bce7-71ee-493a-8474-8d3367b8c387",
          "name": "GenderDetection",
          "request": {
            "url": "http://api.datumbox.com/1.0/GenderDetection.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Gender Detection function identifies if a particular document is written-by or targets-to a man or a woman based on the context, the words and the idioms found in the text."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ce06797-07b9-4ac8-a906-081c1ac3dac6"
            }
          ]
        }
      ]
    },
    {
      "name": "Keyword",
      "item": [
        {
          "id": "c15dbd84-a70a-498b-84cd-b28a60fc981d",
          "name": "KeywordExtraction",
          "request": {
            "url": "http://api.datumbox.com/1.0/KeywordExtraction.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "n",
                  "value": "{}",
                  "disabled": false,
                  "description": "The number of keyword combinations (n-grams) that you wish to extract"
                },
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Keyword Extraction function enables you to extract from an arbitrary document all the keywords and word-combinations along with their occurrences in the text."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "10dc6a44-ea88-419e-bb04-99c18a788aa8"
            }
          ]
        }
      ]
    }
  ]
}