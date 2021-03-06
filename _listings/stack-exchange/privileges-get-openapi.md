---
swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 0
info:
  title: Stack Exchange Get Privileges
  description: "Returns the earnable privileges on a site.\n \nPrivileges define abilities
    a user can earn (via reputation) on any Stack Exchange site.\n \nWhile fairly
    stable, over time they do change. New ones are introduced with new features, and
    the reputation requirements change as a site matures.\n \nThis method returns
    a list of privileges."
  version: "2.0"
host: api.stackexchange.com
basePath: /2.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/privileges:
    get:
      summary: My Priveleges
      description: "Returns the privileges the user identified by access_token has.\n
        \nThis method returns a list of privileges."
      operationId: returns-the-privileges-the-user-identified-by-access-token-has-this-method-returns-a-list-of-privile
      x-api-path-slug: meprivileges-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Privileges
  /privileges:
    get:
      summary: Get Privileges
      description: "Returns the earnable privileges on a site.\n \nPrivileges define
        abilities a user can earn (via reputation) on any Stack Exchange site.\n \nWhile
        fairly stable, over time they do change. New ones are introduced with new
        features, and the reputation requirements change as a site matures.\n \nThis
        method returns a list of privileges."
      operationId: returns-the-earnable-privileges-on-a-site-privileges-define-abilities-a-user-can-earn-via-reputation
      x-api-path-slug: privileges-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Privileges
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