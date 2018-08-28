---
name: Freesound.org
x-slug: freesoundorg
description: Freesound aims to create a huge collaborative database of audio snippets,
  samples, recordings, bleeps, ... released under Creative Commons licenses that allow
  their reuse. Freesound provides new and interesting ways of accessing these samples,
  allowing users to browse the sounds in new ways using keywords, a sounds-like type
  of browsing and more--upload and download sounds to and from the database, under
  the same creative commons license, and interact with fellow sound-artists!
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Freesound_project_website_logo.png
x-kinRank: "8"
x-alexaRank: "6485"
tags: Sounds
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/sounds/master/_listings/freesoundorg/apis.md
specificationVersion: "0.14"
apis:
- name: Freesound Search sounds
  x-api-slug: freesound
  description: This resource allows searching sounds in Freesound by matching their
    tags and other kinds of metadata.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Freesound_project_website_logo.png
  humanURL: https://freesound.org
  baseURL: https://www.freesound.org//apiv2//search/text
  tags: Search, Sounds
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sounds/master/_listings/freesoundorg/searchtext-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sounds/master/_listings/freesoundorg/searchtext-get-openapi.md
- name: Freesound Details of a sound
  x-api-slug: freesound
  description: This resource allows the retrieval of detailed information about a
    sound.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Freesound_project_website_logo.png
  humanURL: https://freesound.org
  baseURL: https://www.freesound.org//apiv2//sounds/{soundId}
  tags: Sounds
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sounds/master/_listings/freesoundorg/soundssoundid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sounds/master/_listings/freesoundorg/soundssoundid-get-openapi.md
- name: Freesound
  x-api-slug: freesound
  description: Freesound aims to create a huge collaborative database of audio snippets,
    samples, recordings, bleeps, ... released under Creative Commons licenses that
    allow their reuse. Freesound provides new and interesting ways of accessing these
    samples, allowing users to browse the sounds in new ways using keywords, a sounds-like
    type of browsing and more--upload and download sounds to and from the database,
    under the same creative commons license, and interact with fellow sound-artists!
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Freesound_project_website_logo.png
  humanURL: https://freesound.org
  baseURL: https://www.freesound.org//apiv2
  tags: Sounds
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sounds/master/_listings/freesoundorg/openapi.md
x-common:
- type: x-blog
  url: https://blog.freesound.org/
- type: x-crunchbase
  url: https://crunchbase.com/organization/freesound
- type: x-developer
  url: https://freesound.org/help/developers/
- type: x-documentation
  url: https://freesound.org/docs/api/
- type: x-forum
  url: https://freesound.org/forum/
- type: x-login
  url: https://freesound.org/home/login/?next=/apiv2/apply/
- type: x-terms-of-service
  url: https://freesound.org/help/tos_web/
- type: x-twitter
  url: https://twitter.com/freesounddev?lang=en
- type: x-website
  url: https://freesound.org
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---