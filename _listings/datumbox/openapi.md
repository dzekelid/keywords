swagger: "2.0"
x-collection-name: Datumbox
x-complete: 1
info:
  title: DatumBox
  description: datumbox-offers-a-machine-learning-platform-composed-of-14-classifiers-and-natural-language-processing-functions--functions-include-sentiment-analysis-topic-classification-readability-assessment-language-detection-and-much-more-
  version: 1.0.0
host: api.datumbox.com
basePath: 1.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /KeywordExtraction.json:
    post:
      summary: Extracts the Keywords of the Document
      description: The Keyword Extraction function enables you to extract from an
        arbitrary document all the keywords and word-combinations along with their
        occurrences in the text.
      operationId: KeywordExtraction
      x-api-path-slug: keywordextraction-json-post
      parameters:
      - in: formData
        name: "n"
        description: The number of keyword combinations (n-grams) that you wish to
          extract
      - in: formData
        name: text
        description: The text that you want to analyze
      responses:
        200:
          description: OK
      tags:
      - Keyword
      - Extraction