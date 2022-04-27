_client_ $\to$ __[[GraphQL#Server]]__
_client_ $\to$ __[[Python#Server]]__
since the python server will have a socket instance of its own 
there is no reason to have the [[GraphQL]] server act as a middle man

instead both servers will share the same database for the python AI to learn from

[[GraphQL#Server]] $\to$ [[MongoDB]] , [[MySQL]]
[[Python#Server]] $\to$ [[MySQL]]