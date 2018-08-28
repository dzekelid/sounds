---
swagger: "2.0"
x-collection-name: CallFire
x-complete: 0
info:
  title: Callfire Download a WAV sound
  description: Download the WAV version of the hosted file. This is an audio data
    endpoint. Returns binary response of the 'audio/mpeg' content type
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /campaigns/sounds:
    get:
      summary: Find sounds
      description: To find all campaign sounds which were created by user. Returns
        all sounds available to be used in campaigns
      operationId: findCampaignSounds
      x-api-path-slug: campaignssounds-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: filter
        description: Name of a file to search for
      - in: query
        name: includeArchived
        description: Includes ARCHIVED sounds for true value
      - in: query
        name: includePending
        description: Includes UPLOAD/RECORDING sounds for true value
      - in: query
        name: includeScrubbed
        description: Includes SCRUBBED sounds for true value
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: offset
        description: Offset to the start of a given page
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - Sounds
  /campaigns/sounds/calls:
    post:
      summary: Add sound via call
      description: Use this API to create a sound via a phone call. Provide the required
        phone number in the CallCreateSound object inside the request, and user will
        receive a call shortly after with instructions on how to record a sound over
        the phone.
      operationId: postCallCampaignSound
      x-api-path-slug: campaignssoundscalls-post
      parameters:
      - in: body
        name: body
        description: Request object containing the name of a new campaign sound and
          phone number to call up
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Limit fields received in response
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - Sounds
      - Calls
  /campaigns/sounds/files:
    post:
      summary: Add sound via file
      description: Create a campaign sound file via a supplied .mp3 or .wav file
      operationId: postFileCampaignSound
      x-api-path-slug: campaignssoundsfiles-post
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: formData
        name: file
        description: A sound file encoded in binary form
      - in: formData
        name: name
        description: Optional name of a sound file, if the name is empty than it will
          be taken from a file
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - Sounds
      - Files
  /campaigns/sounds/tts:
    post:
      summary: Add sound via text-to-speech
      description: 'Use this API to create a sound file via a supplied string of text.
        Add a text in the TextToSpeech.message field, and pick a voice in the TextToSpeech.voice
        field. Available voices are: MALE1, FEMALE1, FEMALE2, SPANISH1, FRENCHCANADIAN1'
      operationId: postTTSCampaignSound
      x-api-path-slug: campaignssoundstts-post
      parameters:
      - in: body
        name: body
        description: textToSpeech
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Limit fields received in response
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - Sounds
      - Tts
  /campaigns/sounds/{id}:
    delete:
      summary: Delete a specific sound
      description: Deletes a single campaign sound instance for a specific campaign
        sound id, this operation does not delete sound completely, it sets sound status
        to ARCHIVED which means that sound will no longer appear in 'find' operation
        results, but still accessible via 'get' operation
      operationId: deleteCampaignSound
      x-api-path-slug: campaignssoundsid-delete
      parameters:
      - in: path
        name: id
        description: An id of a campaign sound
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - Sounds
    get:
      summary: Find a specific sound
      description: Returns a single CampaignSound instance for a given sound id in
        campaign. This is a meta data to the sounds. No audio data is returned from
        this API
      operationId: getCampaignSound
      x-api-path-slug: campaignssoundsid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a sound campaign
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - Sounds
  /campaigns/sounds/{id}.mp3:
    get:
      summary: Download a MP3 sound
      description: Download the MP3 version of a hosted file. This is an audio data
        endpoint. Returns binary response of the 'audio/mpeg' content type
      operationId: getCampaignSoundDataMp3
      x-api-path-slug: campaignssoundsid-mp3-get
      parameters:
      - in: path
        name: id
        description: An id of a campaign sound
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - Sounds.mp3
  /campaigns/sounds/{id}.wav:
    get:
      summary: Download a WAV sound
      description: Download the WAV version of the hosted file. This is an audio data
        endpoint. Returns binary response of the 'audio/mpeg' content type
      operationId: getCampaignSoundDataWav
      x-api-path-slug: campaignssoundsid-wav-get
      parameters:
      - in: path
        name: id
        description: An id of a campaign sound
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - Sounds.wav
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