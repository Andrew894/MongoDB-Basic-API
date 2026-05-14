# MongoDB-Basic-API
## Questions
1. What is the purpose of using `.env`

    To parameterize configurations per enviroment, also stores sensative information like passwords and API keys seperate from the main application. 

2. How does this work:
```js
if (query.minPrice || query.maxPrice) {
    filter.price = {};
    if (query.minPrice) filter.price.$gte = Number(query.minPrice);
    if (query.maxPrice) filter.price.$lte = Number(query.maxPrice);
}
```
`
    This code checks if the user provided either a minimum price or a maximum price in the request, and inside of a filter object creates an empty price. If either a minPrice or a maxPrice exists adds the either     the $lte or $gte operator and converts the value to a number and filters the products that are are within the price range given.

3. What is the program `seed.js` used for?

    `seed.js` is used to populate the database with inital data so the database does not start empty.

4. Try all API routes using Postman
5. In terms of code what is the difference between `put` and `patch`

## Exercise
Do a repo of your own to represent whatever you want as long as it has four fields (data members), make sure that your program has the "same" API routes and to provide test data. The README file should have screenshots of using all API routes, either by using Postman, or by modifying `index.html` to have all the operations. Also, add the answers to the questions on your README.

