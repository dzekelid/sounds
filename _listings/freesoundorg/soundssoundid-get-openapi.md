---
swagger: "2.0"
x-collection-name: Freesound.org
x-complete: 0
info:
  title: Freesound Details of a sound
  description: This resource allows the retrieval of detailed information about a
    sound.
  termsOfService: http://freesound.org/help/tos_api/
  version: 1.0.0
host: www.freesound.org
basePath: /apiv2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search/text:
    get:
      summary: Search sounds
      description: This resource allows searching sounds in Freesound by matching
        their tags and other kinds of metadata.
      operationId: searchText
      x-api-path-slug: searchtext-get
      parameters:
      - in: query
        name: filter
        description: Allows filtering query results
      - in: query
        name: group_by_pack
        description: This parameter represents a boolean option to indicate whether
          to collapse results belonging to sounds of the same pack into single entries
          in the results list
      - in: query
        name: page
        description: Query results are paginated, this parameter indicates what page
          should be returned
      - in: query
        name: page_size
        description: Indicates the number of sounds per page to include in the result
      - in: query
        name: query
        description: The query! The query is the main parameter used to define a query
      - in: query
        name: sort
        description: Indicates how query results should be sorted
      responses:
        200:
          description: OK
      tags:
      - Search
      - Sounds
  /sounds/{soundId}:
    get:
      summary: Details of a sound
      description: This resource allows the retrieval of detailed information about
        a sound.
      operationId: getSoundById
      x-api-path-slug: soundssoundid-get
      parameters:
      - in: path
        name: soundId
        description: ID of the sound that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Sounds
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---