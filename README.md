# claimclam-takehome-assesment
Takehome assesment for a fullstack engineer

## Summary

For this assessment you will be fetching podcasts from a provided api endpoint and rendering them in a list.

Please use this provided endpoint: https://601f1754b5a0e9001706a292.mockapi.io/podcasts

some documentation:
```
SEARCHING
Add query params to GET request:

/podcast?search=Comedy - search by all fields for string Comedy
/podcast?title=The%20Trevor%20Noah%20Podcast - search any field by property name (title)
/podcast?categoryName=History - search any field by property name (categoryName)

PAGINATION
Add query params to GET requests:

/podcats?page=1&limit=10
or /podcasts?p=1&l=10
```

## Requirements

1. Create a controlled input field to fetch podcasts from the given api. By default you should request all podcasts on initial load.

2. Add a debounce of 500ms to avoid fetching on every key press.

3. Render a list of podcasts from the request. Feel free to use any data from the response that you find relevant or necessary to show (Don't worry about styling here yet).

4. Handle UI states for:
- When the podcasts are being fetched.
- When the response returns some podasts.
- When the response returns no podcasts that match the search value.

## Bonus

1. Add some styling to the search results. Feel free to render as a list, cards, etc. Whatever would be a nice UI for the end user.
2. Add some pagination. The api supports "page" and "limit" params.
