# SmartBrain - v3
Final project for ZTM course - Advanced

1. Clone this repo
2. Run `npm install`
3. Run `npm start`
4. You will need to create your own AWS Lambda http endpoint for the ranking badge to work.

Ps, you can learn more about Dockerfile commands by using this resource: https://docs.docker.com/engine/reference/builder/#usage

You can find out more about the 3 commands we just learned here:

[docker-compose build](https://docs.docker.com/compose/reference/build/)

[docker-compose run](https://docs.docker.com/compose/reference/run/)

[docker-compose up](https://docs.docker.com/compose/reference/up/)

To learn more about Volumes in Docker:

https://stackoverflow.com/questions/34809646/what-is-the-purpose-of-volume-in-dockerfile


https://www.linux.com/learn/docker-volumes-and-networks-compose

1. How we set up the database with username and password: (see the environment variables section) https://hub.docker.com/_/postgres/

2. psql  command: https://www.postgresql.org/docs/9.2/static/app-psql.html

# Redis:

key-value - redis
small pieace of data

documents - mongodb, couchdb
large pieases of data

wide coloumn - casandra
large pieases of data

graph - neo4j
large pieases of data

## commands

- GET
- SET
- DEL
- EXISTS
- SET session
- EXPIRE
- INCREBY
- DECR

## data types:

- string

- SET
- GET
- MSET (multiple set)
- MGET (multiple get)

- hash

- HMSET (hash multiple set)
- HGET (hash get)
- HGETALL (hash get all)

- list

- LPUSH (left push)
- RPUSH (right push)
- LRANGE (list range)

- sets

- SADD
- SMEMBERS
- SISMEMBERS

- sorted sets

- ZADD
- ZRANGE
- ZRANK

- Fast database, easy scalable

# JWT and SESSION

## resources:
Cookie based authentication and token based authentication is a complex topic with a lot of opinions. It's always good to learn both sides and understand the pros and cons. I will leave these resources for you to explore, but keep in mind that it is better to come back to these after you have completed this section so you have a better understanding of how everything works. 

1. https://dzone.com/articles/cookies-vs-tokens-the-definitive-guide

2. https://stackoverflow.com/questions/17000835/token-authentication-vs-cookies

3. https://scotch.io/bar-talk/why-jwts-suck-as-session-tokens

Visit the [jwt](jwt.io) website and play around with their JWT interactive page to better understand how everything works before moving on to the next video.

Resources: setState() Callback
There are many times you may want to use a callback function when using setState(). You can read up on the topic a little more in detail here:

1. https://medium.com/@voonminghann/when-to-use-callback-function-of-setstate-in-react-37fff67e5a6c

2. https://stackoverflow.com/questions/42038590/when-to-use-react-setstate-callback

## Exercise: #4 - Improving SmartBrain

Wow, we've really come a long way with the Smart Brain App. However, I bet you noticed many areas that we can improve the application. You see, software is always a constantly evolving journey. As you gain more experience you start to notice areas you can improve the code, and areas you can refactor. This is what you want. It means you are connecting the dots and understanding the information flow between different systems. To continue to practice this skill, I have a few tasks for you. Just like in the real world, there won't be a solution file for you at the end of this one. It either works or it doesn't. Using all you have learned up to this point, using all of your resources (including our community on Discord), see if you can implement these features:



Task 1: Add pet  and age  column to the database and allow users to update these fields on their profile.

Task 2: Implement token flow as we have done so far for /register  end point as well.

Task 3: Add Sign out functionality where you revoke the token when a user signs out of the app

Task 4 (Bonus): You may notice a lot of repeated code (especially when it comes to fetch()). How can you improve this? Try to refactor the code and perhaps also improve the logic to make the app even better!

You can find the github repositories of the code we have worked on up to this point below:
Front End
Back End
Back End - Dockerized

Enjoy the exercise... it's a tough one!

# AWS

- S3
- DynamoDB
- EC2
- Lambda
- CloudFront

## lambda functions:

- serverless ()


# performance

- CDN
    - caching
- GZIP / Brotli
    - decompression
- database scaling
    - indentify inefficient quieries
    - increase memory
    - vertical scaling (redis, memcached)
    - sharding
    - more database
    - database type

# Resources: Caching
To learn more about how caching works and the two headers we discussed in the previous videos: Etag and Cache Control, I recommend you read further using these resources:

1. [Caching Everywhere](https://www.freecodecamp.org/news/the-hidden-components-of-web-caching-970854fe2c49)

2. [Cache Headers](https://web.dev/http-cache/)

3. [Caching and Performance](https://devcenter.heroku.com/articles/increasing-application-performance-with-http-cache-headers)

# load balancer:

- wrk2
- artillery
- siege
- load test (npm package)

# Resources: Nginx
To learn more about the NGINX config file have a look at:  https://nginx.org/en/docs/ and https://www.linode.com/docs/web-servers/nginx/how-to-configure-nginx/

# CI/CD
