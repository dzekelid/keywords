---
name: ParallelDots
x-slug: paralleldots
description: ""
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/paralleldots-logo.png
x-kinRank: "9"
x-alexaRank: ""
tags: Keywords
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/keywords/master/_listings/paralleldots/apis.md
specificationVersion: "0.14"
apis:
- name: ParallelDots Keywords
  x-api-slug: paralleldots
  description: |-
    # Introduction
    What does your API do?

    Keyword Generator are powerful tools in text analysis that can be used to index data, generate tag clouds and accelerate the searching time. It generates an extensive list of relevant keywords and phrases to make research more context focussed.

    # Overview
    Things that the developers should know about

    The API accepts the input parameters as form-data.

    Response will be in JSON as shown below:

    ```
    {
        "keywords": [
            {
                "keyword": "Cristiano Ronaldo",
                "confidence_score": 0.887065
            },
            {
                "keyword": "Principality Stadium",
                "confidence_score": 0.903289
            },
            {
                "keyword": "Cardiff last",
                "confidence_score": 0.806802
            },
            {
                "keyword": "couple",
                "confidence_score": 0.69036
            },
            {
                "keyword": "hours",
                "confidence_score": 0.984956
            },
            {
                "keyword": "Real Madrid win",
                "confidence_score": 0.812151
            }
        ],
        "usage": "By accessing ParallelDots API or using information generated by ParallelDots API, you are agreeing to be bound by the ParallelDots API Terms of Use: http://www.paralleldots.com/terms-and-conditions"
    }
    ```

    # Authentication
    What is the preferred way of using the API?

    An API key is required to be sent as a parameter to authenticate your requests.


    # Rate limit
    Is there a limit to the number of requests an user can send?

    There is no rate limit as such but too many concurrent requests will throw 504 time-out error from nginx.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/paralleldots-logo.png
  humanURL: https://www.paralleldots.com/
  baseURL: https://apis.paralleldots.com//v3//keywords
  tags: Machine Learning,Keywords,Analysis
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keywords/master/_listings/paralleldots/keywords-post-openapi.md
- name: ParallelDots Multilang_Keywords
  x-api-slug: paralleldots
  description: |-
    # Introduction
    What does your API do?

    Extract Keywords from different languages using this API.

    # Overview
    Things that the developers should know about

    The API accepts the input parameters as form-data.The API works best when input long and multiple sentences.Languages supported are German(de), French(fr), Dutch(nl), Italian(it), Spanish(es), Portuguese(pt), Danish(da), Finish(fi)
    Response will be in JSON as shown below:

    ```
    {
        "keywords": [
            {
                "relevance_score": 4,
                "keyword": "Prime Minister Narendra Modi"
            },
            {
                "relevance_score": 6,
                "keyword": "Human Resource Development Minister Smriti Irani"
            },
            {
                "relevance_score": 2,
                "keyword": "Lok Sabha"
            },
            {
                "relevance_score": 1,
                "keyword": "ongoing"
            },
            {
                "relevance_score": 2,
                "keyword": "JNU row"
            },
            {
                "relevance_score": 2,
                "keyword": "Dalit scholar"
            },
            {
                "relevance_score": 2,
                "keyword": "Rohith Vemula"
            },
            {
                "relevance_score": 3,
                "keyword": "Hyderabad Central University"
            }
        ],
        "usage": "By accessing ParallelDots API or using information generated by ParallelDots API, you are agreeing to be bound by the ParallelDots API Terms of Use: http://www.paralleldots.com/terms-and-conditions"
    }

    ```

    # Authentication
    What is the preferred way of using the API?

    An API key is required to be sent as a parameter to authenticate your requests.


    # Rate limit
    Is there a limit to the number of requests an user can send?

    There is no rate limit as such but too many concurrent requests will throw 504 time-out error from nginx.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/paralleldots-logo.png
  humanURL: https://www.paralleldots.com/
  baseURL: https://apis.paralleldots.com//v3//multilang_keywords
  tags: Machine Learning,Multilang_Keywords
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keywords/master/_listings/paralleldots/multilang-keywords-post-openapi.md
- name: ParallelDots
  x-api-slug: paralleldots
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/paralleldots-logo.png
  humanURL: https://www.paralleldots.com/
  baseURL: https://apis.paralleldots.com//v3
  tags: Keywords
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keywords/master/_listings/paralleldots/openapi.md
x-common:
- type: x-blog
  url: https://blog.paralleldots.com/
- type: x-developer
  url: https://www.paralleldots.com/ai-apis
- type: x-documentation
  url: https://docs.paralleldots.com/
- type: x-faq
  url: https://www.paralleldots.com/frequently-asked-questions
- type: x-github
  url: https://github.com/ParallelDots
- type: x-linkedin
  url: https://www.linkedin.com/company/3572541/
- type: x-openapi-gist
  url: https://gist.githubusercontent.com/kinlane/18095af6f37b04ffada94a3378ad9e8b/raw/8ce934fcf5ac1be679873ad12df8ed00b7c750e6/paralleldots-ai-api-openapi.json
- type: x-pricing
  url: https://www.paralleldots.com/pricing
- type: x-terms-of-service
  url: https://www.paralleldots.com/terms-and-conditions
- type: x-twitter
  url: https://twitter.com/ParallelDots
- type: x-website
  url: https://www.paralleldots.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---