# Interactive-Fiction-Engine.c.document

### Overview
```
This repo is the document of Interactive Fiction Engine,
the final project of NTNU_ComputerProgrammingII.
To expereince the project, check out Interactive-Fiction-Engine.c repo in my GitHub.
(The repo may be private until the demo day or deadline)
```

## How did we produced this project

#### Why did we wrote a html frontend and python server and C core system for a project

```
Firstly, since the course are mainly for Freshman to learn C programming,
therefore, the core system are required to be written in C.

However, we considered that SDL for project's GUI is a
little bit ugly and limited for our ideas.
After discussion with teammates, we decided to write a brand new html
user interface for our engine.

At the start of our project, we wrote the whole logic and whole stuff
in frontend and TA told us that it is formidden
since we only use C to generate the html and js,
thus, we wrote a python webserver to connect the frontend and our C system.

According to the rule of project, we have written a complexity C system to
automatically generate frontend codes, including html/js,
by analyzing the script.yaml file.
(Which means our project can automatically generate a whole website according to your script.yaml and assets)

Although it is hard for freshmen, we still do our best to write this wonderful final project.

```

#### How much time did we spend on this project

```
Currently, we've spent more than 100 hours in this project since we really want to
perform and produce a perfect demo. In our opinion, this project may be the biggest project
we have ever written.

Although we have spent a large quantity of time to write this project, bugs may still appear
and we highly encourage developers to send PR or issues to our repo.
```

## Documents of commands

[Server/API/Admin Edit](/doc/server.md)
[Script(Every elements)](/doc/script.md)
