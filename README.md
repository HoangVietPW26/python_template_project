The problem the users need to solve is how best to bring new developers onboard. 

We need to guide our team members in installing the core set of development
tools, creating a working module, and then displaying their completed work at
the end of a sprint. This first project will use the most important tools and assure
that everyone has a common understanding of the tools and the deliverables.

Each developer will build a project to create a small application. This application
will have a command-line interface (CLI) to write a cheerful greeting.

The expectations are shown in the following example:

```
% python src/hello_world.py --who "World"
Hello, World!
```

For initilize docs
```
cd docs
sphinx-quickstart
```

For developers, we often want to install all of the ”extras.” This usually means
executing the following command to create a requirements-dev.txt file that can
be used to build a development environment.
```
% pip-compile --all-extras -o requirements-dev.txt
```
In order to run the tox tool, it’s common to also create a testing-only subset of
the required packages and tools. Use the following command:
```
% pip-compile --extra test -o requirements.txt
```


