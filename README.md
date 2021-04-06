# Daily Kata - Using Spring Boot

## Tasks
 
### Task #1

a. Create an endpoint that persist/save Movie object (POST /movie)

Movie object:
```kotlin
data class Movie(
    val movieId: String,
    val length: Int,
    val watched: Boolean
)
```

b. Create an endpoint that retrieve Movie object by movieId

### Task #2

a. Create an endpoint that persist Availability (e.g. test site availability) 
object (POST /availability)

Availability object:
```kotlin
data class Movie(
    val postCode: String,
    val available: Int,
    val created: Date,
    val lastModified: Date
)
```

b. Create an endpoint that update Availability object (PATCH /availability)

c. Create an endpoint that retrieve Availability object 
(GET /availability/{postCode})

Enrich the data with Suburb and State (NOTE: a postCode can represent multiple
suburb to design the response data class accordingly)

NOTE: you can use this API:
http://v0.postcodeapi.com.au/suburbs/2000.json

### Task #3

... think of something interesting and challenging, but doesn't take longer than 15 minutes ...


## Reminders

1. Always starts by writing test (remember the Red-Green-Refactor cycle)

2. Have at least 1 @WebMvcTest and 1 @SpringBootTest

3. Use flyway (create migration script in db/migration directory) to create tables

4. Use H2 (H2 driver/library already included)

5. Avoid using mouse as much as possible

6. Do this kata regularly and avoid looking up Kotlin syntax or Spring Boot docs
   (maybe not at the first few tries) 

7. And, think of something harder to try and update this README.md

## Inspirations

Inspired by https://osherove.com/tdd-kata-1

> The following is a TDD Kata- an exercise in coding, refactoring and test-first, that you should apply daily for at least 15 minutes .
