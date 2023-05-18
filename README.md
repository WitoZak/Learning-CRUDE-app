
# Movie Library API

This program is a movie library API that provides basic CRUD (Create, Read, Update, Delete) operations for managing movies. It is built using the Spring framework and follows the RESTful architectural style.

## Functionality

The API supports the following operations:

- **GET /movies**: Retrieves a list of all movies in the library.
- **GET /movies/{id}**: Retrieves detailed information about a specific movie identified by its `id`.
- **POST /movies**: Adds one or more movies to the library.
- **PUT /movies/{id}**: Updates the information of a specific movie identified by its `id`.
- **PATCH /movies/{id}**: Partially updates the information of a specific movie identified by its `id`.
- **DELETE /movies/{id}**: Deletes a specific movie from the library identified by its `id`.

The API interacts with a `MovieRepository` class, which handles the persistence of movie data. The `Movie` class represents a movie object and contains properties such as `name` and `rating`.

## Usage

To use the API, you can send HTTP requests to the corresponding endpoints using tools like cURL or Postman. Here are some examples:

- Retrieve all movies:
  ```
  GET /movies
  ```

- Retrieve a specific movie:
  ```
  GET /movies/{id}
  ```

- Add new movies:
  ```
  POST /movies
  Body: [{"name": "Movie 1", "rating": 8.5}, {"name": "Movie 2", "rating": 7.9}]
  ```

- Update a movie:
  ```
  PUT /movies/{id}
  Body: {"name": "Updated Movie", "rating": 9.0}
  ```

- Partially update a movie:
  ```
  PATCH /movies/{id}
  Body: {"rating": 8.7}
  ```

- Delete a movie:
  ```
  DELETE /movies/{id}
  ```
