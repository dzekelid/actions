---
swagger: "2.0"
x-collection-name: Buffer
x-complete: 1
info:
  title: Bufferapp
  description: social-media-management-for-marketers-and-agencies
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
---