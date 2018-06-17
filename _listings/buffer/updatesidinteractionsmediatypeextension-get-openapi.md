---
swagger: "2.0"
x-collection-name: Buffer
x-complete: 0
info:
  title: Buffer Get Updates Interactions Mediatypeextension
  description: Returns the detailed information on individual interactions with the
    social media update such as favorites, retweets and likes.
  version: "1"
host: api.bufferapp.com
basePath: /1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /updates/{id}/interactions{mediaTypeExtension}:
    get:
      summary: Get Updates Interactions Mediatypeextension
      description: Returns the detailed information on individual interactions with
        the social media update such as favorites, retweets and likes.
      operationId: returns-the-detailed-information-on-individual-interactions-with-the-social-media-update-such-as-fav
      x-api-path-slug: updatesidinteractionsmediatypeextension-get
      parameters:
      - in: query
        name: count
        description: Specifies the number of status updates to receive
      - in: query
        name: event
        description: Specifies a type of event to be retrieved, for example retweet,
          like, comment, mention or reshare
      - in: path
        name: id
      - in: path
        name: mediaTypeExtension
      - in: query
        name: page
        description: Specifies the page of status updates to receive
      responses:
        200:
          description: OK
      tags:
      - Updates
      - Id
      - InteractionsmediaTypeExtension
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