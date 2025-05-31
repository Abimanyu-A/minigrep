This is a CLI based query finder from a file

So far basic implementation of taking a filename and reading it's content

Now there are two main things we need to do
1. Maintain modular functions - one responsibility per function
2. Query and filename are connected - But the connection is not established so far
3. Proper error response messages

As for 1. 
Reading the filename and query has been moved to a different function named new() and to implement the coupling between the query and filename struct is used and the new method is a implementation of Config(struct name)

A run function is created to manage the access(reading and printing) of content from a file

The config, and run are put in separate crate named lib.rs for better maintainability and separated logic. 

Creating test driven development