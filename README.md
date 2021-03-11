Backend API for the myFlix application, a movie database/website.

Usage on Postman

Add user first using post method https://radiant-journey-16913.herokuapp.com/users

Log in using post method https://radiant-journey-16913.herokuapp.com/users

Copy the token created

Do this everytime the endpoint is returning a 401 status code meaning you are not authenticated to access the endpoint. On authorization tab select "Bearer Token" and paste the token in the input.

Available endpoints and description

Movie

https://radiant-journey-16913.herokuapp.com/movies - Get all movies

https://radiant-journey-16913.herokuapp.com/movies/:Title - Get movie by title

https://radiant-journey-16913.herokuapp.com/movies/genres/Drama - Get genre by title

https://radiant-journey-16913.herokuapp.com/movies/director/David%20Fincher - Get director by name Users

Awailable user for testing, feel free to create your own

{ "username": "test1",
"password": "test1",
"email": "test@test.com",
"birthday": "11-11-2011"
}

https://radiant-journey-16913.herokuapp.com/director/test1- Update user on the body raw follow the same format as adding use. for example

{ "username": "test1",
"password": "test2",
"email": "test@test.com",
"birthday": "11-11-2011"
}

https://radiant-journey-16913.herokuapp.com/users/test1 - Remove user

https://radiant-journey-16913.herokuapp.com/users/test1/movies/5f96c527f9d625bac874a3c8 - add favorite movie

https://radiant-journey-16913.herokuapp.com/users/test1/movies/5f96c527f9d625bac874a3c8 -remove favorite movie

Authentication

https://radiant-journey-16913.herokuapp.com/users - Login user

Usage

If you clone or download the repo. Replace the connection db with your own connection strings.

// Connect to database

mongoose.connect(process.env.CONNECTION_URI,

{ useNewUrlParser: true, useCreateIndex: true, useFindAndModify: false, useUnifiedTopology: true, }

Install Dependencies

$ npm install

Run App in dev mode

$ npm run dev

Demo The API is live at https://radiant-journey-16913.herokuapp.com/

Version: 1.0.0

License: MIT

Credits: Mitchell Zilbergs
