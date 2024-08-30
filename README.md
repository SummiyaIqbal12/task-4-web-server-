# Simple HTTP Server

This is a basic HTTP server implemented in C++ that serves static HTML files. It is designed to handle multiple client requests concurrently using threads.

## Overview

This HTTP server listens on port 8080 and serves an `index.html` file located in the same directory. If the file is not found, it returns a simple 404 error page.

## Features

- Handles multiple client connections using threads.
- Serves static HTML content.
- Responds with a 404 error page if the requested file is not found.

## Prerequisites

- C++ compiler (e.g., g++, clang++)
- C++ standard library and POSIX libraries
- Basic knowledge of HTTP and networking

## Build and Run

1. **Clone the repository:**

   ```bash
   git clone <repository_url>
   cd <repository_directory>
   ```

2. **Compile the code:**

   ```bash
   g++ -o http_server http_server.cpp -pthread
   ```

   Make sure you replace `http_server.cpp` with the name of your source file if it's different.

3. **Run the server:**

   ```bash
   ./http_server
   ```

   The server will start and listen on port 8080.

4. **Test the server:**

   Open a web browser or use `curl` to test the server:

   ```bash
   curl http://localhost:8080
   ```

   You should see the content of the `index.html` file. If the file is not found, you'll get a 404 error page.

## File Structure

- `http_server.cpp`: The main source file for the HTTP server.
- `index.html`: The HTML file served by the server (create this file as needed).

## Notes

- Ensure the `index.html` file is present in the same directory as the executable. If you wish to serve different files or handle different types of requests, modifications to the code will be necessary.
- This server is for educational purposes and is not intended for production use.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For questions or suggestions, please contact [your_email@example.com](mailto:your_email@example.com).

---
