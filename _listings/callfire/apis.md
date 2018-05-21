---
name: CallFire
x-slug: callfire
description: CallFire is a cloud-based telephony company that provides voice and text
  connectivity services. It offers the necessary tools for businesses to communicate
  and market effectively. The company works to provide a diverse line of innovative
  products that enable its users to get their messages delivered.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/CallFire_Logo.png
x-kinRank: "9"
x-alexaRank: ""
tags: Sounds
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/sounds/master/_listings/callfire/apis.md
specificationVersion: "0.14"
apis:
- name: Callfire Find sounds
  x-api-slug: callfire
  description: To find all campaign sounds which were created by user. Returns all
    sounds available to be used in campaigns
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/CallFire_Logo.png
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//campaigns/sounds
  tags: Campaigns,Sounds
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sounds/master/_listings/callfire/campaignssounds-get-openapi.md
- name: Callfire Add sound via call
  x-api-slug: callfire
  description: Use this API to create a sound via a phone call. Provide the required
    phone number in the CallCreateSound object inside the request, and user will receive
    a call shortly after with instructions on how to record a sound over the phone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/CallFire_Logo.png
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//campaigns/sounds/calls
  tags: Campaigns,Sounds,Calls
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sounds/master/_listings/callfire/campaignssoundscalls-post-openapi.md
- name: Callfire Add sound via file
  x-api-slug: callfire
  description: Create a campaign sound file via a supplied .mp3 or .wav file
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/CallFire_Logo.png
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//campaigns/sounds/files
  tags: Campaigns,Sounds,Files
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sounds/master/_listings/callfire/campaignssoundsfiles-post-openapi.md
- name: Callfire Add sound via text-to-speech
  x-api-slug: callfire
  description: 'Use this API to create a sound file via a supplied string of text.
    Add a text in the TextToSpeech.message field, and pick a voice in the TextToSpeech.voice
    field. Available voices are: MALE1, FEMALE1, FEMALE2, SPANISH1, FRENCHCANADIAN1'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/CallFire_Logo.png
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//campaigns/sounds/tts
  tags: Campaigns,Sounds,Tts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sounds/master/_listings/callfire/campaignssoundstts-post-openapi.md
- name: Callfire Delete a specific sound
  x-api-slug: callfire
  description: Deletes a single campaign sound instance for a specific campaign sound
    id, this operation does not delete sound completely, it sets sound status to ARCHIVED
    which means that sound will no longer appear in 'find' operation results, but
    still accessible via 'get' operation
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/CallFire_Logo.png
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//campaigns/sounds/{id}
  tags: Campaigns,Sounds
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sounds/master/_listings/callfire/campaignssoundsid-delete-openapi.md
- name: Callfire Find a specific sound
  x-api-slug: callfire
  description: Returns a single CampaignSound instance for a given sound id in campaign.
    This is a meta data to the sounds. No audio data is returned from this API
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/CallFire_Logo.png
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//campaigns/sounds/{id}
  tags: Campaigns,Sounds
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sounds/master/_listings/callfire/campaignssoundsid-get-openapi.md
- name: Callfire Download a MP3 sound
  x-api-slug: callfire
  description: Download the MP3 version of a hosted file. This is an audio data endpoint.
    Returns binary response of the 'audio/mpeg' content type
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/CallFire_Logo.png
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//campaigns/sounds/{id}.mp3
  tags: Campaigns,Sounds.mp3
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sounds/master/_listings/callfire/campaignssoundsidmp3-get-openapi.md
- name: Callfire Download a WAV sound
  x-api-slug: callfire
  description: Download the WAV version of the hosted file. This is an audio data
    endpoint. Returns binary response of the 'audio/mpeg' content type
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/CallFire_Logo.png
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//campaigns/sounds/{id}.wav
  tags: Campaigns,Sounds.wav
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sounds/master/_listings/callfire/campaignssoundsidwav-get-openapi.md
- name: Callfire
  x-api-slug: callfire
  description: CallFire is a cloud-based telephony company that provides voice and
    text connectivity services. It offers the necessary tools for businesses to communicate
    and market effectively. The company works to provide a diverse line of innovative
    products that enable its users to get their messages delivered.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/CallFire_Logo.png
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2
  tags: Sounds
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sounds/master/_listings/callfire/openapi.md
x-common:
- type: x-net-sdk
  url: https://github.com/CallFire/CallFire-CSharp-SDK
- type: x-account-billing
  url: https://answers.callfire.com/hc/en-us/sections/200166268-Billing
- type: x-account-settings
  url: https://answers.callfire.com/hc/en-us/sections/200187056-Account-Settings
- type: x-authentication
  url: https://www.callfire.com/api-documentation/how-do-i-enable-api-on-my-account
- type: x-blog
  url: https://www.callfire.com/blog
- type: x-blog-rss
  url: https://www.callfire.com/blog/feed
- type: x-twitter
  url: https://twitter.com/CallFire
- type: x-case-studies
  url: https://www.callfire.com/case-studies
- type: x-compliance
  url: https://www.callfire.com/legal/compliance
- type: x-contact-form
  url: https://www.callfire.com/contact
- type: x-crunchbase
  url: https://www.crunchbase.com/organization/callfire
- type: x-developer
  url: https://www.callfire.com/api-documentation
- type: x-documentation
  url: https://www.callfire.com/api-documentation/rest/version/1.1
- type: x-drupal-plugin
  url: https://github.com/CallFire/CallFire-Drupal-Integration
- type: x-email
  url: support@callfire.com
- type: x-facebook
  url: https://www.facebook.com/callfire
- type: x-faq
  url: https://answers.callfire.com/hc/en-us/sections/200193833-FAQs
- type: x-getting-started
  url: https://www.callfire.com/help/docs/getting-started
- type: x-github
  url: https://github.com/callfire
- type: x-glossary
  url: https://www.callfire.com/help/glossary/communications
- type: x-google-plus
  url: https://plus.google.com/100142045997033051154
- type: x-messages
  url: https://www.callfire.com/ui/number/messages?6
- type: x-partners
  url: https://www.callfire.com/partners
- type: x-phone
  url: 1.877.897.3473
- type: x-php-sdk
  url: https://github.com/CallFire/CallFire-PHP-SDK
- type: x-pricing
  url: https://www.callfire.com/pricing
- type: x-privacy
  url: https://www.callfire.com/legal/privacy
- type: x-selfservice-registration
  url: https://www.callfire.com/ui/register?1
- type: x-terms-of-service
  url: https://www.callfire.com/legal/terms
- type: x-tickets
  url: https://answers.callfire.com/hc/en-us/requests/new
- type: x-tour
  url: javascript:;
- type: x-videos
  url: https://answers.callfire.com/hc/en-us/articles/200849247-Videos
- type: x-webinars
  url: https://answers.callfire.com/hc/en-us/articles/202174798-Webinars
- type: x-website
  url: http://www.callfire.com
- type: x-wordpress-plugin
  url: https://github.com/CallFire/CallFire-WordPress-Integration
- type: x-youtube
  url: https://www.youtube.com/user/CallFireTelephony
- type: x-zapier
  url: https://zapier.com/zapbook/callfire/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---