# MongoDB-Basic-API
What is the purpose of using .env
How does this work:
if (query.minPrice || query.maxPrice) {
    filter.price = {};
    if (query.minPrice) filter.price.$gte = Number(query.minPrice);
    if (query.maxPrice) filter.price.$lte = Number(query.maxPrice);
}
What is the program seed.js used for?
Try all API routes using Postman
In terms of code what is the difference between put and patch
