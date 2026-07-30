**As a** user  
**I need** to view all available gifts  
**So that** I can browse and choose a gift to request.

### Details and Assumptions

* Gifts are stored in the MongoDB database.
* The API endpoint `/api/gifts` returns all available gifts.
* Users can view gifts without logging in.

### Acceptance Criteria

```gherkin
Given the GiftLink application is running
When the user sends a GET request to `/api/gifts`
Then the API returns a list of all available gifts with a status code of 200

Given there are gifts stored in the database
When the user opens the gifts page
Then all available gifts are displayed to the user
```
