# Week 5 Notes

## Graphs

Quite often a good visualisation or representation of a problem will make it easier to solve.  A common solution is a simple graph - where we have vertices or nodes (representing things) and edges between them (representing connections).

Think about the "6 degrees of Kevin Bacon" theory.  We can have each actor represented by a vertex and each movie they share with another actor represented by an edge between vertices.

## The 7 Bridges of Koenigsberg

In this puzzle, discussed by Euler, you are asked whether you could go over all seven bridges in Koenigsberg and return to your original starting point.

This is a classic example of a problem begging to be represented by a graph.  So each land mass is a vertex and each bridge is an edge.

You can then do trial and error.  Can you trace your way across all the lines in the graph and return to where you started.

You quickly notice that one of the main patterns is that when you start from a point and go back to it then leave it again you are left with no remaining bridges back to the point.  Or you could try to go back to it at the end, but then the last bridge takes you away.

How can we explain this mathematically?  Each vertex has an odd number of edges.  The number of edges that connect to a vertex is called the degree of that vertex.  So we can say that each vertex has an odd degree.

By logic, we can state, that in order to end at our starting point in a graph we need to start from a vertex with an even degree.  The Koenigsberg bridge problem is therefore impossible.

## Do even degrees on each vertex imply a Euler Circuit is possible?

A 'Euler Circuit' is what we were looking for in Keonigsberg Bridge problem - a route over all of the edges of a graph that ends where it starts.

We have ruled out the possibility of a Euler Circuit where all vertices have an odd degree.

In fact, we can extend this and say that if any vertex has an odd degree a Euler Circuit is impossible.  Since we have to use all possible edges from that vertex, we will either get stuck on that vertex or not use all of its connections.

So what if all our vertexes have even degree - will we always end where we start?  Yes - but why?  Think about our first move - after this move there is only one vertex with an odd edge (our original starting point).  Consider this as our starting point.  If we now tried to make a Euler circuit we'd fail and we'd always fail on our original vertex.

We have started by moving randomly through a graph where each vertex has an even degree.  What approach can we follow that could improve likelihood of success at finding a Euler circuit?

We could start by working on top of our original graph - what if we start from a vertex that has already been touched and has remaining unused edges and repeat the random movement process.  We've created another circuit.  How do we put the two circuits together?  In the first circuit, when we reach the vertex we move on the second circuit and then when we get back to the beginning, we go back to the original circuit.  We now have a much larger circuit.  We could do this ad infinitum and eventually build a Euler circuit.  Will we always build a Euler circuit?  Yes - because we're always left with a smaller test case of the same problem, we're always going to be able to make a circuit.



