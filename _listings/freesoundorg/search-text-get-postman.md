{
  "info": {
    "name": "Freesound Search sounds",
    "_postman_id": "b0ede66d-096c-487c-9cb3-8f443cdc5996",
    "description": "This resource allows searching sounds in Freesound by matching their tags and other kinds of metadata.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "search",
      "item": [
        {
          "id": "0fcf2b52-3e54-4b3f-818a-0d421e494da1",
          "name": "searchText",
          "request": {
            "url": "http://www.freesound.org/apiv2/search/text?filter=%7B%7D&group_by_pack=%7B%7D&page=%7B%7D&page_size=%7B%7D&query=%7B%7D&sort=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This resource allows searching sounds in Freesound by matching their tags and other kinds of metadata"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0956340-cee5-4825-8207-64b57bc3e6d9"
            }
          ]
        }
      ]
    }
  ]
}