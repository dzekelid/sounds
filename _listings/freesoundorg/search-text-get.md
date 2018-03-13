---
swagger: "2.0"
info:
  title: Freesound
  description: With the Freesound APIv2 you can browse, search, and retrieve information
    about Freesound users, packs, and the sounds themselves of course. You can find
    similar sounds to a given target (based on content analysis) and retrieve automatically
    extracted features from audio files, as well as perform advanced queries combining
    content analysis features and other metadata (tags, etc...). With the Freesound
    APIv2, you can also upload, comment, rate and bookmark sounds!
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
        their tags and other kinds of metadata
      operationId: searchText
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
      - search
      - sounds
definitions:
  Sound:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      url:
        description: This is a default description.
        type: get
x-collection-name: Freesound.org
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