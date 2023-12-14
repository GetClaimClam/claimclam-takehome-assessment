# claimclam-takehome-assesment
Takehome assessment for a fullstack engineer position

## Summary

Imagine that you have a podcasts microservice (please see API spec below). For this assessment you need to create a gateway service that will be utilizing podcast service and create a UI for it.


some documentation:
```
Service URL: https://601f1754b5a0e9001706a292.mockapi.io
API Spec
Add query params to GET request:
/podcasts - get all podcasts (https://601f1754b5a0e9001706a292.mockapi.io/podcasts)
/podcasts?search=Comedy - search by all fields for string Comedy
/podcasts?title=The%20Trevor%20Noah%20Podcast - search any field by property name (title)
/podcasts?categoryName=History - search any field by property name (categoryName)

PAGINATION
Add query params to GET requests:

/podcats?page=1&limit=10
or /podcasts?p=1&l=10
```

## Requirements
Backend(golang preffered):
1. Create an api-gateway service for podcasts microservice with basic error handling and input validation functions

UI(next.js preffered):
1. Create a controlled input field to fetch podcasts. By default you should request all podcasts on initial load.

2. Add a debounce of 500ms to avoid fetching on every key press.

2. Render a list of podcasts from the request. Feel free to use any data from the response that you find relevant or necessary to show (Don't worry about styling here yet).

3. Handle UI states for:
- When the podcasts are being fetched.
- When the response returns some podasts.
- When the response returns no podcasts that match the search value.

## Bonus

1. Add some styling to the search results. Feel free to render as a list, cards, etc. Whatever would be a nice UI for the end user.
2. Add some pagination. The api supports "page" and "limit" params.
3. Add a debounce of 500ms to avoid fetching on every key press.
4. Use graphQL as a protocol between UI and API gateway
5. Add basic rate limiting and heartbeat features to API gateway
   
