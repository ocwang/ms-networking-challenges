# Basic Networking Challenges
### Monday, Feb. 13th

**Context:** A client wants to build a simple wrapper around Product Hunt using the PH API. The first feature the client wants you to implement is a feed that displays all of today's featured products. The client wants to keep the project lean and asks you explicitly not to use any dependencies or third party libraries.

**Specs:**

1. Create your URL in a composable manner so the client can easily add more features reusing base URL and/or adding more parameters to existing URLs.

2. Add unit tests verifying the scheme, host, path, base URL, query of the URL.

3. Make a networking request to fetch all of the products featured today on PH.

4. Convert the data returned into models using flatMap and failable initializers.

5. Display the data returned in a feed that shows each product's name, tagline, number of votes, and thumbnail.

6. If a user clicks on a post, show a new screen with all the comments for that post, sorted in descending order.

7. After you've completed steps 1-6, go back and refactor your code so that you're constructing URL requests with an enum.

**Resources:**
https://api.producthunt.com/v1/docs/

You will need to sign up for Product Hunt, register an application, and generate a token.

Example:

Name: PHAPIExampleApp

Redirect URI: http://localhost:3000/users/auth/producthunt/callback

# Intermediate Networking Challenges
### Wednesday, Feb. 15th

###### Challenge 1
**Context:** After arguing for a couple days, you're finally able to convinence the client to see the value in Alamofire. You'll be switching your networking layer from using Apple's native URLSession to Alamofire. Because you've built your app to be modular, you're able to easily replace URLSession with Alamofire.

After switching to AF, the client has given you a new set of requests.

**Specs**

1. Once you scroll to the end of the listed products, the client wants to paginate to see the previous day's products.

2. Implement a better way of handling async image-loading and caching.

3. Better security and handling of headers and auth token.

4. Handle common network errors.

5. Unfortunately PH doesn't give us write access, but implement upvote / unvote functionality on client side.

6. After completing steps 1-4, reflect over the implementation of your network layer and see if you can refactor it to be better.
