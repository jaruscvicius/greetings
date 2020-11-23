# greetings

A RESTful web service for study purposes

## Running

### Option 1:

**Build and execute:**

`mvn spring-boot:run`

### Option 2:

**Build an executable JAR:**

`mvn clean package`

**Run the JAR file:**

`java -jar target/greetings-0.0.1-SNAPSHOT.jar`

## Testing the Service

Now that the service is up, visit `http://localhost:5000/greeting`, where you should see:

```json
{"id":1,"content":"Hello, World!"}
```

If provided a `name` query string parameter (e.g.: `http://localhost:5000/greeting?name=User`), the value
of the content attribute will change from `Hello, World!` to `Hello, User!`, as the following listing shows:

```json
{"id":1,"content":"Hello, User!"}
```
