[Previously... on StackOverflow...](http://stackoverflow.com/q/42357785/878701)

## The setup

1. Create two .Net Core projects (**A** & **B**) in two *separate* solutions in the same folder.  From **A**, create a Nuget package.  (You can upload it to Nuget, MyGet, or just keep locally.  Just make sure the source is configured.)

2. In **B**, add the Nuget package.

## The result

Project **A** has now been added to the solution for Project **B**.

## The questions

1. Why is this happening?
2. How can I get VS to recognize that it should be referencing the Nuget package, not the project?

## Other stuff

I'm running VS 2015 Pro Update 3 on Windows 10.

In my real scenario, my Nuget package is at a later version.  When I open the *project.json* file, I get a compiler warning on the `ProjectA` dependency that says I'm depending on version 1.1, but version 1.0 is found.

I'm working on an example and will link to it once done.