# ASCII Art Web Application

  

This Go code provides a simple web server that generates ASCII art based on user inputs. It allows users to input text and select a banner type, then generates ASCII art based on the chosen banner. The server utilizes HTTP methods to handle both GET and POST requests.

## Functionality

1. Setting Up

  

The server listens on http://localhost:8080.

It serves static files from the /static directory.

  

2. Handling Requests

  

### GET Request:

Loads the main HTML template (index.html) to the root URL (/).

Displays a form for user input.

  

### POST Request:

Processes form data containing input text and the selected banner type.

Generates ASCII art based on the user's input.

Logs the input data, selected banner type, and the resulting ASCII art.

Redirects the user back to the main page (/?) with the output displayed.

  

## Usage

Running the Server

  

Download or clone the repository containing this code.

Execute the following command in the terminal:

  

go run main.go

  

Access the server at http://localhost:8080 in a web browser.

  

## Using the Web Interface

  

Access http://localhost:8080.

Enter text in the input field.

Choose a banner type from the provided options.

Submit the form to generate the corresponding ASCII art.

The resulting ASCII art will be displayed on the same page.

  

## Dependencies

  

The code depends on the following:

Go standard library.

External package html/template for HTML templating.

  

## File Structure

  

main.go: Contains the main code handling the HTTP server and request processing.

templates/index.html: HTML template for the web interface.

static/: Directory containing static files served by the server.

  

## Important Notes

  

Ensure that the necessary templates and static files are present in the correct directories for proper functionality.

The server will log input data and generated ASCII art in the console for monitoring.

  

Link to [Audit](https://github.com/01-edu/public/tree/master/subjects/ascii-art-web/audit).

## DOCKER 
Use next commands to run docker
```
docker build -t ascii-art-web-dockerize .

docker run -p 8080:8080 ascii-art-web-dockerize
```