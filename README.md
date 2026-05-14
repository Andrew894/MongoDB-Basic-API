# MongoDB-Basic-API
## Questions
1. What is the purpose of using `.env`

To parameterize configurations per environment, also stores sensitive information like passwords and API keys separately from the main application. 

2. How does this work:
```js
if (query.minPrice || query.maxPrice) {
    filter.price = {};
    if (query.minPrice) filter.price.$gte = Number(query.minPrice);
    if (query.maxPrice) filter.price.$lte = Number(query.maxPrice);
}
```

This code checks if the user provided either a minimum price or a maximum price in the request, and inside of a filter object, creates an empty price. 
If either a minPrice or a maxPrice exists adds either the $lte or $gte operator and converts the value to a number, and filters the products that are within the price range given.

3. What is the program `seed.js` used for?

`seed.js` is used to populate the database with inital data so the database does not start empty.

5. Try all API routes using Postman

In terms of code what is the difference between `put` and `patch`

## Exercise
Do a repo of your own to represent whatever you want, as long as it has four fields (data members), make sure that your program has the "same" API routes and to provide test data. 
The README file should have screenshots of using all API routes, either by using Postman, or by modifying `index.html` to have all the operations. Also, add the answers to the questions on your README.

<img width="1090" height="976" alt="API-Books_GET" src="https://github.com/user-attachments/assets/95abe190-7ef2-4d50-93a9-f5082e249ef4" />
<img width="1208" height="816" alt="API-Books_POST" src="https://github.com/user-attachments/assets/47ebb109-682b-45c0-b8b1-a521dfb13be4" />
<img width="1137" height="832" alt="API-Books_PUT" src="https://github.com/user-attachments/assets/fccd220a-9f06-41ab-ae45-8a68bef441a1" />
<img width="1152" height="797" alt="API-Books_PATCH" src="https://github.com/user-attachments/assets/aa9adc70-c77a-4876-9fe1-93357ea0bf1a" />
<img width="1147" height="707" alt="API-Books_DELETE" src="https://github.com/user-attachments/assets/a0a71334-c9ea-4b89-b7f8-7287f9aab264" />
