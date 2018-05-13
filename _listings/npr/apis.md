---
name: NPR
description: NPR delivers breaking national and world news. Also top stories from
  business, politics, health, science, technology, music, arts and culture. Subscribe
  to podcasts and RSS feeds.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/141-npr.jpg
x-kinRank: "9"
x-alexaRank: "641"
tags:
- Stack Network
- Stack
- Radio
- Publishing
- News
- Mobile
- Media
- Getting Started
- Federal Government
- Broadcasting
created: "2018-03-27"
modified: "2018-03-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/authorization/master/_listings/npr/apis.yaml
specificationVersion: "0.14"
apis:
- name: NPR
  description: NPR delivers breaking national and world news
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/141-npr.jpg
  humanURL: ""
  baseURL: https://api.npr.org//
  tags: Authorization
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/authorization/master/_listings/npr/authorization-v2-token-revoke-post.md
- name: NPR Show a web-based login/signup form to a user
  description: |-
    If the parameters passed to this endpoint are correct, it will redirect to `npr.org/oauth2/login` for the user to complete the sign-in.

    Currently acceptable values for `scope` are any combination of the following:
    - `identity.readonly` - for read-only access to the Identity Service
    - `identity.write` - for write access to the Identity Service
    - `listening.readonly` - for read-only access to the Listening Service
    - `listening.write` - for write access to the Listening Service
    - `localactivation` - for all access to the Local Activation Service

    It is generally suggested that you assume that you will need all of the current scopes in order to successfully implement an NPR One application.

    If the parameters passed in are NOT correct and the client passed in a valid `redirect_uri` parameter, the request will be redirected to `{{YOUR_REDIRECT_URI}}?error={{ERROR_TYPE}}&message={{ERROR_DESCRIPTION}}`.
    If the parameters passed are NOT correct and the client did not pass in a valid `redirect_uri` parameter, this endpoint will return the errors encoded as JSON objects (along with the corresponding HTTP status code -- usually 400).
    The latter is intended for development and debugging purposes -- in a real-world situation, errors returned as JSON objects are irretrievable by the client application, and thus passing in a valid `redirect_uri` is critical even for the purpose of capturing errors.

    If the user successfully logs in and authorizes the application, the request will be redirected to `{{YOUR_REDIRECT_URI}}?code={{AUTHORIZATION_CODE}}&state={{CSRF_TOKEN}}`

    If the user DENIES the application, they will be redirected to `{{YOUR_REDIRECT_URI}}?error=denied&message=The%20user%20has%20denied%20the%20login%20and%20access%20request&state={{CSRF_TOKEN}}`.
    This means that if your application flow requires a user to log in in order to proceed, it is up to you to give them the proper messaging explaining that the sign-in must be authorized in order to continue.

    Finally, please do not confuse an authorization code with an access token. Once your app has completed this flow, you will still need to call `POST /authorization/v2/token` in order to swap the code for a valid access token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/141-npr.jpg
  humanURL: http://www.npr.org
  baseURL: https://api.npr.org//
  tags: Authorization
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/authorization/master/_listings/npr/authorization-v2-authorize-get.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/authorization/master/_listings/npr/authorization-v2-authorize-get-postman.md
x-common:
- type: x-base
  url: http://api.npr.org/
- type: x-codecademy
  url: http://www.codecademy.com/tracks/npr
- type: x-crunchbase
  url: https://crunchbase.com/organization/npr
- type: x-crunchbase
  url: http://www.crunchbase.com/company/npr
- type: x-developer
  url: http://dev.npr.org/
- type: x-documentation
  url: http://dev.npr.org/#accessing-the-api
- type: x-email
  url: permissions@npr.org
- type: x-email
  url: ogcstaff@npr.org
- type: x-email
  url: employment@npr.org
- type: x-email
  url: careers@npr.org
- type: x-email
  url: kroc@npr.org
- type: x-email
  url: mediarelations@npr.org
- type: x-email
  url: sponsorship@npr.org
- type: x-email
  url: ashamblin@npr.org
- type: x-email
  url: giving@npr.org
- type: x-email
  url: giftplanning@npr.org
- type: x-getting-started
  url: http://dev.npr.org/#quick-start
- type: x-github
  url: https://github.com/npr
- type: x-selfservice-registration
  url: http://www.npr.org/templates/reg/
- type: x-terms-of-service
  url: http://www.npr.org/about-npr/179876898/terms-of-use
- type: x-twitter
  url: https://twitter.com/NPR
- type: x-twitter
  url: https://twitter.com/NPRTechTeam
- type: x-website
  url: http://www.npr.org
- type: x-base
  url: http://api.npr.org/
- type: x-codecademy
  url: http://www.codecademy.com/tracks/npr
- type: x-crunchbase
  url: https://crunchbase.com/organization/npr
- type: x-crunchbase
  url: http://www.crunchbase.com/company/npr
- type: x-developer
  url: http://dev.npr.org/
- type: x-documentation
  url: http://dev.npr.org/#accessing-the-api
- type: x-email
  url: permissions@npr.org
- type: x-email
  url: ogcstaff@npr.org
- type: x-email
  url: employment@npr.org
- type: x-email
  url: careers@npr.org
- type: x-email
  url: kroc@npr.org
- type: x-email
  url: mediarelations@npr.org
- type: x-email
  url: sponsorship@npr.org
- type: x-email
  url: ashamblin@npr.org
- type: x-email
  url: giving@npr.org
- type: x-email
  url: giftplanning@npr.org
- type: x-getting-started
  url: http://dev.npr.org/#quick-start
- type: x-github
  url: https://github.com/npr
- type: x-selfservice-registration
  url: http://www.npr.org/templates/reg/
- type: x-terms-of-service
  url: http://www.npr.org/about-npr/179876898/terms-of-use
- type: x-twitter
  url: https://twitter.com/NPR
- type: x-twitter
  url: https://twitter.com/NPRTechTeam
- type: x-website
  url: http://www.npr.org
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---