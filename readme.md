Reflection Questions

1. What was the most "painful" part of building this without a framework?

kind of choatic and messy and so many code should input than when we have framework that we just put the code and git push it

2. Why do you think we need to manually collect "chunks" of data in the POST route?

if i input new chunk task to my code the post request will collected it peice by peice and collect and complete the data

3. What HTTP status code did we return when a task was successfully created, and why?

the status code is "201 created" standard that tell the client that the task is succesfully added to new resource server


4. If you had to add a DELETE route, what would the code look like? (Write a short pseudo-code snippet.)

this is javascript

if (request.method === "DELETE" && pathname.startsWith("/tasks/")) {

    id = extractId(pathname);


    deleteTask(id);

    response.writeHead(200, { "Content-Type": "application/json" });
    response.end(JSON.stringify({ message: "Task deleted successfully" }));
}