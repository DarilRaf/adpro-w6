<h2>Commit 1 Reflection notes</h2>
What does the handle_connection() method does?

The handle\*connection() method takes TcpStream as a parameter which is mutable so that the method could read from and write to this stream.
Then, BufReader is added to add buffering to the read operations on the stream.
After that, it declares the http*request variable as a Vec<*> which is like an enum array that contains the buf_reader where it reads all the line from the incoming HTTP request until it reached an empty line.
Finally, it calls the println! macro to print the http request into the console.
