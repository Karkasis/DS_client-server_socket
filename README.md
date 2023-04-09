# DS_client-server_socket
Short Description
Simulates the operation of a network database for the storage and management of films using Java Socket technology

Full Description
Implementation of a distributed system that
follows the client-server model and concerns a system that simulates the
operation of a network database for the storage and management of films
making use of Java Socket technology to communicate between entities
their. The application consists of a server to which many will connect
clients (users) but not at the same time (i.e. your implementation should not do
thread usage). The client and server should only exchange
objects.
The client application, through an appropriate graphical environment, will have the ability
to make requests to import new movies and to search by title
of the film (consider it unique) or the director. In the case of searching with
based on the director the films that will satisfy the specific criterion can be
more than one.

The storage and management of the films is undertaken by the server which
has an object file for permanent storage on disk as well as dynamic structures
data for faster processing in memory (choose the most efficient structures for
the temporary storage of the data). The information that should be recorded for
each movie is: its title, director, movie genre, duration in minutes
and a little description about the premise of the film.

Communication between client and server follows a specific protocol. THE
The client application first sends a BEGIN message to the server to start
the handshake. The server responds with a LISTENING message. Then he sends
client the type of request (INSERT or SEARCH) and the data concerning it
specific request. For its part, the server takes the appropriate actions
actions to satisfy the request.In the case of a search request o
server sends the tape(s) information or NORECORD message to the client
since there is no relevant record that satisfies the search request, while in
import request case stores the received record. With success
completion of its actions, the server sends the OK message to the client. Finally o
client sends the END message and terminates the connection.

The programs must check every phase of it
protocol that they received the correct message. Otherwise they must interrupt
the connection.
