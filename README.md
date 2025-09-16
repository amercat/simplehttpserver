# HTTP Parser in Java

This project is a minimal HTTP request parser implemented in Java.  
It takes raw HTTP requests from an input stream and converts them into structured objects.

## Project Content

- **HttpRequest** → Represents an HTTP request (method, target, version).
- **HttpParser** → Reads from an input stream and extracts the request line, headers, and body.
- **HttpMethod** → Enum for supported HTTP methods.
- **HttpMessage** → Base class for HTTP messages.
- **HttpParserTest** → Unit test with a valid HTTP request example.

## Test Phase

A test is provided (`HttpParserTest`) using JUnit 5.  
It creates a raw HTTP request, passes it through the parser, and validates that the request line and headers are parsed correctly.

You can run it from your IDE or with Maven/Gradle.  
When executed, the test ensures that:

- The HTTP method (`GET`) is parsed.
- The request target (`/`) is parsed.
- The HTTP version (`HTTP/1.1`) is parsed.
- Headers are read and available.

## How to Run

1. Clone the repository.
2. Open in IntelliJ (or your favorite IDE).
3. Run `HttpParserTest`.

