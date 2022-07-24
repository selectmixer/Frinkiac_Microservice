# FRINKIAC - RANDOM SIMPSONS IMAGE MICROSERVICE 

This microservice will provide a random image still from the TV show Simpsons, along with the corresponding metadata for that still (episode, airdate, etc.).

This microservice server can be run on localhost, with a specified port (default: 8080).
When called, the server will retrieve data from the required Frinkiac API and return a random image link, + corresponding metadata, as a JSON object.



### DEPENDENCIES

Node, Express, Axios




### HOW TO REQUEST DATA

A user or project can retrieve the data needed using a simple get request to the specified port (default:8080).
For example, when this microservice is running, a user or project can access `localhost:8080/` in a browser to request data. Alternatively, if working with RESTful app, something like axios can be implemented and the data can be fetched with “axios.get(“localhost:8080”) “




### HOW TO RECEIVE DATA

When a user or project requests data as above, the microservice will automatically return as a response a random image link + metadata, in JSON. The JSON object will have the following keys:

>Episode, Timestamp, Title, Director, Writer, Airdate, Image, Subtitles

- ‘Image’ will be a URL to the image.

- ‘Subtitles’ will be an array of strings.

- ‘Timestamp’ will be an integer.

- Everything else will be a string.

This response can be viewed, stored or used by a user in a variety of different ways by the user or project accessing this data. For example, the JSON object can be stored in a variable and accessed.
