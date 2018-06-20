{
  "info": {
    "name": "Global Change Information System API Redirect to a particular publication.",
    "_postman_id": "3bb7c0e5-7f7c-413b-96d0-dba543cfd747",
    "description": "Given a numeric ID, redirect to the full URI of a publication.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activities",
      "item": [
        {
          "id": "e9da8118-513e-4e3a-974b-3c82c48daded",
          "name": "list-the-activities-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/activity?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the activities, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7efb7fac-a977-46e1-9a33-8123f0e0c638"
            }
          ]
        }
      ]
    },
    {
      "name": "Representation",
      "item": [
        {
          "id": "107f6526-18aa-49a8-977b-38a66195da63",
          "name": "get-json-which-represents-the-structure-of-an-activity",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "activity/:activity_identifier"
              ],
              "variable": [
                {
                  "id": "activity_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of an activity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ead1488-2597-4d7f-9fcd-a866c2a61b55"
            }
          ]
        },
        {
          "id": "c4247b3a-d9ec-44f1-ae6b-523a59059392",
          "name": "get-json-which-represents-the-structure-of-an-array",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "array/:array_identifier"
              ],
              "query": [
                {
                  "key": "with_gcmd",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "with_regions",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "array_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of an array."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cecbb954-6aae-47e7-8f30-3c8f6fa9ea00"
            }
          ]
        },
        {
          "id": "505591b5-4f11-40a6-8437-9a7af0d77ac9",
          "name": "get-json-which-represents-the-structure-of-an-article",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "article/:article_identifier"
              ],
              "query": [
                {
                  "key": "with_gcmd",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "with_regions",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "article_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of an article."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5541f6a7-6ab3-4db9-abe5-a8303bc2ea3c"
            }
          ]
        },
        {
          "id": "badcf45e-37de-46ad-9ad1-a746905bbfff",
          "name": "get-json-which-represents-the-structure-of-a-book",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "book/:book_identifier"
              ],
              "query": [
                {
                  "key": "with_gcmd",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "with_regions",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "book_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a book."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8200761-53dc-440c-92c2-64f635f00885"
            }
          ]
        },
        {
          "id": "23d315ed-e8af-4c9a-be76-e79426951886",
          "name": "get-json-which-represents-the-structure-of-a-dataset",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "dataset/:dataset_identifier"
              ],
              "variable": [
                {
                  "id": "dataset_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a dataset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f6e5e09-3d82-4a43-a9b7-1b03651d57c7"
            }
          ]
        },
        {
          "id": "13badca0-b92f-4b0d-8f72-f8361bbeb39b",
          "name": "get-json-which-represents-the-structure-of-a-file",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "file/:file_identifier"
              ],
              "variable": [
                {
                  "id": "file_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "de8fd7dc-b38e-43f1-8740-5989e680c7b1"
            }
          ]
        },
        {
          "id": "9f39c772-cbcf-4172-9489-cd6a387595cc",
          "name": "get-json-which-represents-the-structure-of-a-gcmd-keyword",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "gcmd_keyword/:gcmd_keyword_identifier"
              ],
              "variable": [
                {
                  "id": "gcmd_keyword_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a GCMD keyword."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b26a6ab4-2fe6-4b6d-a602-5da825b00ce8"
            }
          ]
        },
        {
          "id": "82396d85-cb9f-448b-bd97-43284a875d4e",
          "name": "get-json-which-represents-the-structure-of-a-generic-publication",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "generic/:generic_identifier"
              ],
              "variable": [
                {
                  "id": "generic_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a generic publication."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92580825-f6ec-4a5c-b9d2-d85dd9181d1e"
            }
          ]
        },
        {
          "id": "25ba05a1-5eaf-4a93-9893-7c756d8e4631",
          "name": "get-json-which-represents-the-structure-of-an-image",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "image/:image_identifier"
              ],
              "query": [
                {
                  "key": "with_gcmd",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "with_regions",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "image_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of an image."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4727657-556d-4f13-8049-1d161b56fbfa"
            }
          ]
        },
        {
          "id": "989efbed-569c-4a6a-87cd-9c9262e94df2",
          "name": "get-json-which-represents-the-structure-of-an-instrument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "instrument/:instrument_identifier"
              ],
              "variable": [
                {
                  "id": "instrument_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of an instrument."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58120808-66ff-4b6a-b883-e5cced2105e5"
            }
          ]
        },
        {
          "id": "e93fcf51-e135-487c-a83d-46aec896b483",
          "name": "get-json-which-represents-the-structure-of-a-journal",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "journal/:journal_identifier"
              ],
              "variable": [
                {
                  "id": "journal_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a journal."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f636288f-2116-4bf0-b9f9-e9723168ec88"
            }
          ]
        },
        {
          "id": "dd1c94a1-8493-44d3-b281-4b9b55db48ef",
          "name": "get-json-which-represents-the-structure-of-a-lexicon",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "lexicon/:lexicon_identifier"
              ],
              "variable": [
                {
                  "id": "lexicon_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a lexicon."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f205fa68-8f75-490b-816f-5830328523c0"
            }
          ]
        },
        {
          "id": "9f44f053-d23a-478c-9c2e-a4f2441c11d5",
          "name": "get-json-which-represents-the-structure-of-a-model",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "model/:model_identifier"
              ],
              "variable": [
                {
                  "id": "model_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a model."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47a654cf-5cbd-47ef-9fe2-02589da58913"
            }
          ]
        },
        {
          "id": "47ec4727-141a-4795-81d7-fd2b6db521fc",
          "name": "get-json-which-represents-the-structure-of-a-model-run",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "model_run/:model_identifier/:scenario_identifier/:range_start/:range_end/:spatial_resolution/:time_resolution/:sequence"
              ],
              "variable": [
                {
                  "id": "model_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "range_end",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "range_start",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "scenario_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sequence",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "spatial_resolution",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "time_resolution",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a model run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ded3bb54-bd1c-46bc-8b83-36726d1b175c"
            }
          ]
        },
        {
          "id": "a29f6edf-b381-49d3-b9f1-1969c0256bb2",
          "name": "get-json-which-represents-the-structure-of-a-model-run",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "model_run/:model_run_identifier"
              ],
              "variable": [
                {
                  "id": "model_run_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a model run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f22bdc85-2dde-45ec-af23-3b41192e8229"
            }
          ]
        },
        {
          "id": "39ce1f48-8a0d-4b4f-a964-b483c2fdea50",
          "name": "get-json-which-represents-the-structure-of-an-organization",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "organization/:organization_identifier"
              ],
              "variable": [
                {
                  "id": "organization_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33b27f74-9cf0-4aa9-8208-8a382e48a03c"
            }
          ]
        },
        {
          "id": "8694e691-4458-4d21-8a5d-2f0997dc49d8",
          "name": "get-json-which-represents-the-structure-of-a-person",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "person/:person_identifier"
              ],
              "variable": [
                {
                  "id": "person_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a person."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b7674a38-61e3-4785-8125-c435b2bb557b"
            }
          ]
        },
        {
          "id": "eca13973-6ae0-4688-8b2e-734fccbf60fd",
          "name": "get-json-which-represents-the-structure-of-a-platform",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "platform/:platform_identifier"
              ],
              "variable": [
                {
                  "id": "platform_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a platform."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70760b3e-a3de-498f-a903-30638ec74567"
            }
          ]
        },
        {
          "id": "30e33716-446a-4665-8fe3-3d2016543d28",
          "name": "get-json-which-represents-the-structure-of-an-instrument-on-a-platform",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "platform/:platform_identifier/instrument/:instrument_identifier"
              ],
              "variable": [
                {
                  "id": "instrument_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "platform_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of an instrument on a platform."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4319ddc-a53d-428e-a289-05b180620fb6"
            }
          ]
        },
        {
          "id": "651fd36b-373c-4a6b-844b-2771f0f9ff5d",
          "name": "get-json-which-represents-the-structure-of-a-project",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "project/:project_identifier"
              ],
              "variable": [
                {
                  "id": "project_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get JSON which represents the structure of a project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "565aed2a-0469-470f-b3df-0f56e2ecd65e"
            }
          ]
        }
      ]
    },
    {
      "name": "Arrays",
      "item": [
        {
          "id": "c58bcfe0-05de-4039-84f6-e93610cbd8d3",
          "name": "list-the-arrays-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/array?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the arrays, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f923d8b-59f3-44d6-91fb-fab7bbcc90c2"
            }
          ]
        }
      ]
    },
    {
      "name": "Articles",
      "item": [
        {
          "id": "91cfb19b-06c8-4829-8a36-91c2450f8e6a",
          "name": "list-the-articles-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/article?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the articles, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0094c5e6-1f7e-4e69-9830-22794f40795b"
            }
          ]
        }
      ]
    },
    {
      "name": "Books",
      "item": [
        {
          "id": "ad23108e-3996-4e7b-9844-59c6b254ddd6",
          "name": "list-the-books-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/book?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the books, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "217e5e40-de18-4601-b16e-0a8531c250da"
            }
          ]
        }
      ]
    },
    {
      "name": "Redirect",
      "item": [
        {
          "id": "e6fb8e42-eb54-4228-8a33-1278ba216f47",
          "name": "given-a-numeric-id-redirect-to-the-full-uri-of-a-contributor",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "contributor/:contributor_identifier"
              ],
              "variable": [
                {
                  "id": "contributor_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a numeric ID, redirect to the full URI of a contributor."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aac661bb-1ea9-45c4-a857-fedc7650e68e"
            }
          ]
        },
        {
          "id": "53862522-3474-4486-adf5-1b8c63817a87",
          "name": "given-a-name-case-sensitive-concatenated-by-dashes-redirect-if-there-is-a-single-match--the-first-an",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "person/:name"
              ],
              "variable": [
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a name (case sensitive, concatenated by dashes), redirect if there is a single match.  The first and last names can be in either order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ab6b0f2-c5b2-4101-907b-8ae3acfe2b98"
            }
          ]
        },
        {
          "id": "f903b33f-886a-41ef-98cb-982498631e5f",
          "name": "given-an-orcid-if-there-is-a-match-redirect-to-the-persons-uri",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "person/:orcid"
              ],
              "variable": [
                {
                  "id": "orcid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given an ORCID, if there is a match, redirect to the persons URI."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8524dac-ffb6-4684-b320-faf8c10621a9"
            }
          ]
        },
        {
          "id": "39554206-51fa-4937-8b4f-7999e99b7e44",
          "name": "given-a-numeric-id-redirect-to-the-full-uri-of-a-publication",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "publication/:publication_identifier"
              ],
              "variable": [
                {
                  "id": "publication_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a numeric ID, redirect to the full URI of a publication."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3588076-ca59-41f0-abc1-575cc18a0c14"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "97424f5d-626d-46a8-9d6a-7b9f388102be",
          "name": "list-the-datasets-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/dataset?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the datasets, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37eca372-e940-4698-ab64-e511ad479911"
            }
          ]
        }
      ]
    },
    {
      "name": "Look",
      "item": [
        {
          "id": "3e56db41-0954-44b6-8888-0803b5eeea83",
          "name": "given-a-doi-return-a-redirect-to-the-gcis-dataset",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "dataset/lookup/:doi"
              ],
              "variable": [
                {
                  "id": "doi",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a DOI, return a redirect to the GCIS dataset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2977a3e-5386-4a9b-920f-bb4b6672188e"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "11abb9d2-2246-45aa-a5bd-665694af5ecb",
          "name": "list-all-the-figures-in-gcis",
          "request": {
            "url": "http://data.globalchange.gov/figure?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all the figures in GCIS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27506fb9-fc4f-44b1-a7c6-6e826608a94b"
            }
          ]
        }
      ]
    },
    {
      "name": "GCMD",
      "item": [
        {
          "id": "b7230942-36f1-47b4-b117-1ebed62f59b9",
          "name": "list-the-gcmd-keywords-in-the-gcis-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/gcmd_keyword?page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the GCMD keywords in the GCIS, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be5ae092-f3d6-4107-bff3-b61429426e3d"
            }
          ]
        }
      ]
    },
    {
      "name": "Generic",
      "item": [
        {
          "id": "6f762072-785b-4f74-a0d2-7d479d15c3cf",
          "name": "list-the-generic-publications-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/generic?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the generic publications, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2cd4f896-cea2-48f7-9b48-167955475995"
            }
          ]
        }
      ]
    },
    {
      "name": "Images",
      "item": [
        {
          "id": "768a3ff3-088d-4eed-8a47-ec2fe8540222",
          "name": "list-the-images-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/image?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the images, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0200586-1481-475b-8020-8e373e1fdab6"
            }
          ]
        }
      ]
    },
    {
      "name": "Instruments",
      "item": [
        {
          "id": "1964e4da-2ea5-416e-ab97-5426ae921a63",
          "name": "list-the-instruments-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/instrument?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the instruments, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46244414-35c2-41d3-84ac-0886b84b9d5f"
            }
          ]
        },
        {
          "id": "ee458684-b9bb-4ee2-b0bd-82e894082429",
          "name": "list-the-instruments-on-a-platform-20-per-page",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "platform/:platform_identifier/instrument"
              ],
              "query": [
                {
                  "key": "all",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "platform_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the instruments on a platform, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "635e3830-c6f9-401c-8365-474855290d9f"
            }
          ]
        }
      ]
    },
    {
      "name": "Journals",
      "item": [
        {
          "id": "2036b9eb-2320-4eab-b420-74b65c70799c",
          "name": "list-the-journals-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/journal?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the journals, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d25ce75-f3bb-4ec7-8581-f4d12e4695c3"
            }
          ]
        }
      ]
    },
    {
      "name": "Lexicons",
      "item": [
        {
          "id": "73fcce00-626e-4545-b717-7a88dd16dabb",
          "name": "list-the-lexicons-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/lexicon?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the lexicons, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e99c5cbc-ad69-4b50-9a5d-381de4478fbb"
            }
          ]
        }
      ]
    },
    {
      "name": "Lookup",
      "item": [
        {
          "id": "f721166d-22cf-4e8a-b982-4e7aac226808",
          "name": "given-a-lexicon-term-and-context-return-a-303-redirect-to-a-gcid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "lexicon/:lexicon_identifier/find/:context/:term"
              ],
              "variable": [
                {
                  "id": "context",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "lexicon_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "term",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a lexicon, term, and context, return a 303 redirect to a GCID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "089a16d1-6ecd-4043-af09-187408050c72"
            }
          ]
        },
        {
          "id": "14f6a0a6-6717-4878-b693-e03f7e2663fd",
          "name": "given-a-lexicon-term-and-context-return-a-303-redirect-to-a-gcid1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "lexicon/:lexicon_identifier/:context/:term"
              ],
              "variable": [
                {
                  "id": "context",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "lexicon_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "term",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a lexicon, term, and context, return a 303 redirect to a GCID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76146308-42ba-47b5-980e-f2a115f4fcf1"
            }
          ]
        }
      ]
    },
    {
      "name": "Terms",
      "item": [
        {
          "id": "87dfe886-e416-4cee-aa50-8d5ed5128a87",
          "name": "list-the-terms-within-a-context-of-a-lexicon",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "lexicon/:lexicon_identifier/list/:context"
              ],
              "variable": [
                {
                  "id": "context",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "lexicon_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the terms within a context of a lexicon"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c49a1380-19d9-4b77-89ce-52043116cfb0"
            }
          ]
        }
      ]
    },
    {
      "name": "Overall",
      "item": [
        {
          "id": "e8c6317b-665a-4a26-9936-a79a1e478a99",
          "name": "get-overall-metrics-about-gcis-data",
          "request": {
            "url": "http://data.globalchange.gov/metrics",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get overall metrics about GCIS data"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b95b9687-30f7-41ac-b559-9ba496ba939b"
            }
          ]
        }
      ]
    },
    {
      "name": "Models",
      "item": [
        {
          "id": "e8baed55-d8a7-4717-8ed6-1a74d3878153",
          "name": "list-the-models-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/model?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the models, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d60a5cdb-9364-4b32-8aef-b7eeb7ae292e"
            }
          ]
        }
      ]
    },
    {
      "name": "Model",
      "item": [
        {
          "id": "7714f099-4a8e-41f4-ad8a-b8a27975db1c",
          "name": "list-the-model-runs-for-a-particular-model-20-per-page",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "model/:model_identifier/run"
              ],
              "query": [
                {
                  "key": "all",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "model_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the model runs for a particular model, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99bd6843-3302-4fda-9355-302c9c552591"
            }
          ]
        },
        {
          "id": "e674875b-2af2-4d43-b7b1-1ed4353b3280",
          "name": "list-the-model-runs-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/model_run?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the model runs, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e40be73c-0c6b-4572-a2f1-985b1f7ec268"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizations",
      "item": [
        {
          "id": "b9e69936-1a49-4345-8576-be9c45064b9e",
          "name": "list-the-organizations-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/organization?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the organizations, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76ec904e-f02c-4b4f-bd42-03020d65e129"
            }
          ]
        }
      ]
    },
    {
      "name": "Show",
      "item": [
        {
          "id": "f9d34455-c751-4166-aa37-58c1538c8324",
          "name": "given-a-resource-dataset-report-etc-and-a-role-editor-etc-and-an-identifier-for-an-organization-show",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "organization/:organization_identifier/contributions/:role_type_identifier/:resource"
              ],
              "variable": [
                {
                  "id": "organization_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resource",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "role_type_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a resource (dataset, report, etc.) and a role (editor, etc), and an identifier for an organization, show the resources to which the organization has contributed in that role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e357f28-ce25-4fed-9cf5-3812561bd5e0"
            }
          ]
        },
        {
          "id": "301cde80-725f-4ed0-a0e7-4435105b8e74",
          "name": "given-a-resource-dataset-report-etc-and-a-role-editor-etc-and-an-identifier-for-a-person-show-the-re",
          "request": {
            "url": {
              "protocol": "http",
              "host": "data.globalchange.gov",
              "path": [
                "person/:person_identifier/contributions/:role_type_identifier/:resource"
              ],
              "variable": [
                {
                  "id": "person_identifier",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resource",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "role_type_identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a resource (dataset, report, etc.) and a role (editor, etc), and an identifier for a person, show the resources to which the person has contributed in that role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3201098-8b29-42a4-bad8-8cc718d157c5"
            }
          ]
        }
      ]
    },
    {
      "name": "People",
      "item": [
        {
          "id": "3b27bb62-d636-4d2a-9995-35dfe9b2efb9",
          "name": "list-the-people-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/person?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the people, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d2edb53-eead-4921-a792-4ba5522502c8"
            }
          ]
        }
      ]
    },
    {
      "name": "Platforms",
      "item": [
        {
          "id": "7746ed04-c324-459e-b591-f8d4ed630237",
          "name": "list-the-platforms-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/platform?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the platforms, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6582c010-9d13-4bb1-b60a-6c345b09fdbb"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "0630f77f-e451-4e1f-8787-ba15dd30afc7",
          "name": "list-the-projects-20-per-page",
          "request": {
            "url": "http://data.globalchange.gov/project?all=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the projects, 20 per page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db041116-3e7c-4d7e-865b-22db64b5cc5d"
            }
          ]
        }
      ]
    }
  ]
}