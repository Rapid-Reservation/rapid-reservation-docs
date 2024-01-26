# Design

## Development Stack

We have chose to use the following tech stack:

- Front End / UI: React (Possibly Next.js (react based))
- Backend / API:TBD
- Database: Postgres
- Deployment:TBD
- Hosting:TBD

## Why seperate UI and API?

Seperation of concerns is used alot in production enviroments. Having both the UI(front end) and API (backend) as seperate entities keeps the set of problems isolated. It is also helpful when working on a project, the UI folks can mock data and still build out components without the API. The API team can make sure the endpoints work and return relevant data. Once both side have a "finished" product, its matter of working together to determine what each endpoint should return and how the component will handle the information! Again, it sounds weird conceptually, but in practice it's actually really nice!

## React

React's primary goal is to minimize the bugs that occur when developers are building UIs. It does this through the use of components — self-contained, logical pieces of code that describe a portion of the user interface. These components can be composed together to create a full UI, and React abstracts away much of the rendering work, leaving you to concentrate on the UI design.

**Why React for RR?**
From an industry standpoint, react is the most popular way for Front End design. As this project is an capstone, and a way to show off what we have learned throughout WTCC, we want to show potential employers we undersand industry trends and are able to learn. React also has THE best tutorial and has a very low skill floor/barrier to entry, but a HIGH ceiling, making it accessible and viable for any developer!

The best part is your write a component once, you never write it again! you design a button, you save it as a button component, and when you need a button, you just add that component and can customize the props as you see fit! It sounds weird at first, but watch the tutorial video or check out the docs and it will ALL make sense, I promise!

### Guides and Tutorials

Here are some helpful guides for getting started with React:

- [Getting Started](https://react.dev/learn)
- [React: Tic Tac Toe](https://react.dev/learn/tutorial-tic-tac-toe): Can be done in an hour and REALLY layouts the foundation needed for scope of this projet! If you can do this, you are good to go!
- [Ultimate React Course with Mosh](https://www.youtube.com/watch?v=SqcY0GlETPk)

- [React-Example](https://github.com/Rapid-Reservation/React-Example): I built a simple example React project that create restaraunt tablet that on button click we mark it as open or reserved to give you guys an example that correlates with our project!

## API

For the backend, we will using an API to interact with database and retrieve information. For example, will have a `/api/foo/bar/Menu` endpoint that when hit, will return a JSON object of the whole menu, which we can then use React to take in endpoint, break it down and display in a menu format! This is up for debate, as there is very little javascript taught at Wake Tech, and while the Front End will be using Javascript, alot of actuall component design is HTML, which we have used, and the rest is easy to pick up. Designing an entire api in JS/TS might be out of scope for this project simple because of time to complete - time to learn. The other thought would be to use FastAPI or Flask as the API, which are both python! We have all taken python so there is less learning so easier for people to get started. This is something we will discuss in our first few meetings to figure out where we want to go!

### Guides and Tutorials

Here are some helpful guides for getting started with APIS:

- [Getting Started with Fast API](https://fastapi.tiangolo.com/tutorial/)
- [Getting Started with Flask](https://flask.palletsprojects.com/en/3.0.x/quickstart/)
- [What is an API?](https://www.ibm.com/topics/api)
- [FASTAPI and Flask based CRUD API](https://dev.to/alexmercedcoder/building-full-crud-rest-apis-with-flask-fastapi-using-psychopg2-2k1n)
- [Video: Simple REST API in Flask](https://www.youtube.com/watch?v=zsYIw6RXjfM)
- [Video: Simple Rest API in FastAPI](https://www.youtube.com/watch?v=iWS9ogMPOI0)
- [Video: Simple Rest API in Typescript/Javascript](https://www.youtube.com/watch?v=i8xHOrPP3NA)

## Postgres

We will be using postgres for our database. PostgreSQL is a popular open-source relational database with numerous benefits for developers, including feature availability, standards compliance, community support, and project governance.

Setting up databases are a pain, especially when you essentialy are setting them up one for dev, and one for prod. An EASY way to skip all of this uses our friend [Docker](https://www.docker.com/) to make it easy for us. We will be using `docker-compose` in order to quickly spin up a working database. Everything is managed in the docker compose file and it will spin it up for us. We then just its URL in the .env and BOOM, you are connected! I will have an example of this to show HOW easy and simple it is!

### Guides and Tutorials

Here are is some information on Postgres:

- [Why is PostgreSQL so popular?](https://dev.to/maimoonaabid/why-is-postgresql-getting-so-popular-4o7m)
- [Setting up Postgres DB with Docker Compose!](https://www.youtube.com/watch?v=qECVC6t_2mU)

## Supplmental Technology

- [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)
- [Docker](https://www.docker.com/)

### MORE COMING SOON
