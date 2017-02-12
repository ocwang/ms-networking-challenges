# Basic Networking Challenges
### Monday, Feb. 13th

*Content:* A client wants to build a simple wrapper around Product Hunt using the PH API. The first feature you are to implement is to build a main feed that display's all of today's featured products. The client doesn't want to add any dependencies and asks you explicitly not to use any third party libraries.

*Specs:*

1. Create your URL in a composable manner so the client can easily add more features reusing base URL and/or adding more parameters to existing URLs.

2. Add unit tests verifying the scheme, host, path, base URL, query of the URL.

3. Make a networking request to fetch all of the products featured today on PH.

4. Convert the data returned into models using flatMap and failable initializers.

5. Display the data returned in a feed that shows each product's name, tagline, number of votes, and thumbnail.

6. Add a button so that users can vote and unvote products in the feed.


