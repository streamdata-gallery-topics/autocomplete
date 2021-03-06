---
swagger: "2.0"
x-collection-name: Reddit
x-complete: 0
info:
  title: Reddit Get Subreddit Autocomplete V2
  description: boolean value
  version: 1.0.0
host: www.reddit.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subreddit_autocomplete:
    get&nbsp;:
      summary: Get Subreddit Autocomplete
      description: |-
        Return a list of subreddits and data for subreddits whose names start
        with &#39;query&#39;.
      operationId: get&nbsp;SubredditAutocomplete
      x-api-path-slug: subreddit-autocomplete-getnbsp
      parameters:
      - in: query
        name: include_over_18
        description: boolean value
        type: string
      - in: query
        name: include_profiles
        description: boolean value
        type: string
      - in: query
        name: query
        description: a string up to 50 characters long, consisting of printable characters
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subreddit
      - Autocomplete
  /subreddit_autocomplete_v2:
    get&nbsp;:
      summary: Get Subreddit Autocomplete V2
      description: boolean value
      operationId: get&nbsp;SubredditAutocompleteV2
      x-api-path-slug: subreddit-autocomplete-v2-getnbsp
      parameters:
      - in: query
        name: include_over_18
        description: boolean value
        type: string
      - in: query
        name: include_profiles
        description: boolean value
        type: string
      - in: query
        name: limit
        description: 'an integer between 1 and 10 (default: 5)'
        type: string
      - in: query
        name: query
        description: a string up to 50 characters long, consisting of printable characters
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subreddit
      - Autocomplete
      - V2
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