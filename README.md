# Commit 1 Reflection Notes:
The handle_connection method reads HTTP requests from a Transmission Control Protocol (TCP) stream. A buffered reader `buf_reader` is instantiated to read lines from the stream. These lines are saved into a vector object called `http_request`. The method outputs the collected HTTP request lines.
![alt text](./images/commit2.png)

# Commit 2 Reflection Notes:
`status_line` defines itself for the HTTP response. `contents` defines the body of the HTTP response. `length` gets the length of the contents. `reponse` constructs the response using `status_line`, `contents`, and `length`. `write_all()` writes the response back to the TCP stream.