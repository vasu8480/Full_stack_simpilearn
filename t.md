#what is Full Stack
Full stack is a combination of front end and back end technologies. Full stack developers are responsible for both client and server-side development. They are proficient with HTML, CSS, and JavaScript on the client-side, and with Node.js, Python, Ruby, Java, .NET, PHP, and databases like MySQL or MongoDB on the server-side.

#what is git?
Git is a version control system that is used to track changes to files, particularly code. It is a distributed version control system, which means that it allows multiple developers to work on the same codebase simultaneously and merge their changes together

git client server - it is a client server architecture. The client is the git command line tool that you use to interact with the repository. The server is the git repository that stores the files and the history of changes to those files. The server is usually hosted on a remote machine, but it can also be hosted locally.

some of the git commands are:
git init - Create an empty Git repository or reinitialize an existing one
git add - Add file contents to the index
git commit - Record changes to the repository
git push -u origin master - pushes the changes in your local repository up to the remote repository you specified as the origin
git pull - Fetch from and integrate with another repository or a local branch
git clone - Clone a repository into a new directory
git status - Show the working tree status
git branch - List, create, or delete branches
git checkout - Switch branches or restore working tree files
git merge - Join two or more development histories together
git remote - Manage set of tracked repositories
git reset - Reset current HEAD to the specified state
git log --pretty=oneline - Show commit logs in one line
git revert - Reverts a commit


#What is Angular?
Angular is a front-end web development framework that is mainly used to build single-page applications (SPAs). It is a comprehensive JavaScript framework that was developed and maintained by Google.

features of angular:
1. Angular is a framework for building client applications in HTML and JavaScript.
2. Angular is a platform for building mobile and desktop web applications.
3. Angular is written in TypeScript. It implements core and optional functionality as a set of TypeScript libraries that you import into your apps.
4.Angular is a platform, a framework and a collection of libraries.
5.Document Object Model (DOM) is a tree structure of HTML elements. Angular extends the DOM with additional functionality.
6.Data binding is the automatic synchronization of data between the model and view components. There are four forms of data binding in Angular: interpolation, property binding, event binding, and two-way data binding.
7.Testing is an important part of the development cycle and Angular provides testing libraries and tools to facilitate testing.

#What is Bootstrap?
Bootstrap is a free and open-source CSS framework directed at responsive, mobile-first front-end web development. It contains CSS- and JavaScript-based design templates for typography, forms, buttons, navigation and other interface components.

#What is Node.js?
Node.js is an open-source, cross-platform, JavaScript runtime environment that executes JavaScript code outside a web browser. Node.js lets developers use JavaScript to write command line tools and for server-side scripting—running scripts server-side to produce dynamic web page content before the page is sent to the user's web browser.

It is also commonly used for building real-time applications, such as chat applications and online games, due to its ability to handle multiple connections concurrently.

node.js events:
Node.js is an event-driven platform. Node.js works on the event loop model. It means that Node.js is always ready to perform a task and never waits for an event to occur. Node.js has multiple in-built events available through events module and EventEmitter class which are used to bind events and event-listeners as follows:

#What is Express.js?
its a flexible Node.js web application framework that provides a robust set of features for web and mobile applications. It facilitates the rapid development of Node based Web applications. 


What is npm?
npm is a package manager for the JavaScript programming language. It is the default package manager for the JavaScript runtime environment Node.js. It consists of a command line client, also called npm, and an online database of public and paid-for private packages, called the npm registry.


#What is MySQL?
MySQL is a free and open-source relational database management system (RDBMS) that uses Structured Query Language (SQL) to manage and manipulate data stored in databases.

Basic MySQL commands:
1. CREATE DATABASE - creates a new database
2. CREATE TABLE - creates a new table
3. INSERT INTO - inserts new data into a table
4. SELECT - extracts data from a database
5. UPDATE - updates data in a database
6. DELETE - deletes data from a database
7. ALTER TABLE - changes the structure of a table
8. DROP TABLE - deletes a table

What is maven?
Apache Maven is a build automation tool for Java-based projects. It is used to manage the build, reporting, and documentation of a project.

Maven uses a declarative approach, where the developer specifies what the project should do, and Maven handles the rest. This is achieved through the use of "project object model" (POM) files, which contain the configuration and requirements for a project.

Some key features of Maven include:
1.Dependency management: Maven allows developers to manage project dependencies (libraries and   other external components) in a centralized location.

2.Build life cycle: Maven defines a standard set of phases for the build process, such as compile, test, and package.

3.Plugins: Maven uses plugins to extend its functionality. There are plugins available for a wide variety of tasks, such as compiling code, running tests, and generating documentation.

what is jenkins?
Jenkins is an open-source continuous integration (CI) and continuous delivery (CD) tool written in Java. It is used to automate the build, test, and deployment processes of software projects.

Jenkins allows developers to automatically build, test, and deploy their code changes, ensuring that the code is always in a deployable state. It is often used in conjunction with version control systems, such as Git, to track code changes and trigger automated builds and tests.

Some key features of Jenkins include:

1.Plugins: Jenkins has a large ecosystem of plugins that can be installed to extend its functionality. There are plugins available for a wide variety of tasks, such as building and testing code, deploying to different environments, and integrating with other tools.

2.Pipeline as code: Jenkins allows developers to define their build, test, and deployment processes in code, using a domain-specific language called "Groovy." This allows developers to version control their CI/CD processes and make them reusable across multiple projects.

3.Scalability: Jenkins can be run on a single machine or on a distributed system with multiple agents, allowing it to scale to meet the needs of large projects.

What is selenium?
Selenium is a free (open source) automated testing suite for web applications across different browsers and platforms. It is a portable framework for testing web applications. Selenium provides a playback tool for authoring tests without learning a test scripting language (Selenese). It also provides a test domain-specific language (Selenese) to write tests in a number of popular programming languages, including C#, Groovy, Java, Perl, PHP, Python, Ruby and Scala.
Selenium consists of several components:

Selenium WebDriver: This is the main component of Selenium, which allows developers to control a web browser through code. It provides a set of APIs (Application Programming Interfaces) for different web browsers, such as Chrome, Firefox, and Safari.

1.Advantages of Selenium webdriver:
Compatibility: Selenium WebDriver supports a wide range of web browsers, including Chrome, Firefox, Safari, Edge, and Internet Explorer. This allows developers to test their web applications on a variety of different browsers.

2.Language support: Selenium WebDriver supports a number of programming languages, including Java, Python, C#, and Ruby. This allows developers to choose the language that they are most comfortable with.

3.Community support: Selenium is an open-source tool with a large community of users and developers. This means that there is a wealth of knowledge and support available online, as well as a wide variety of plugins and extensions.

4.Ease of use: Selenium WebDriver has a simple and intuitive API, making it easy for developers to get started with automating web browsers.

Selenium Grid: This component allows developers to run Selenium tests in parallel on multiple machines and across different environments, such as different operating systems and web browsers.

Selenium IDE: This is a browser extension that allows developers to record and replay their interactions with a web application. It is useful for creating quick tests and prototyping.

What is docker?
Docker is a tool for packaging and deploying applications in lightweight containers. Containers allow developers to package an application and its dependencies into a single, self-contained unit that can be easily deployed and run on any platform.
Some key features of Docker include:

Isolation: Containers isolate applications from each other and from the host operating system, ensuring that applications run consistently in different environments.

Portability: Docker allows developers to package an application and its dependencies into a single, self-contained unit that can be easily moved between different environments.

Scalability: Docker allows developers to run multiple containers on a single host, making it easy to scale applications horizontally.

Basic Docker commands:
1.docker run - creates and runs a container
2.docker ps - lists running containers
3.docker images - lists all images
4.docker exec - executes a command in a running container
5.docker stop - stops a running container
6.docker rm - removes a container
7.docker rmi - removes an image
8.docker build - builds an image from a Dockerfile
9.docker login - logs into a Docker registry
10.docker push - pushes an image to a Docker registry

what is docker-compose?
Docker Compose is a tool for defining and running multi-container Docker applications. It allows developers to define a set of services in a YAML file, and then run those services with a single command.

what is docker swarm?
Docker Swarm is a native clustering tool for Docker. It allows developers to create a cluster of Docker hosts and expose it as a single virtual Docker host. This makes it easy to deploy and manage applications on a cluster of Docker hosts.

what is docker deamon?
The Docker daemon (dockerd) is a background service running on the host that manages building, running, and distributing Docker containers. The Docker daemon exposes a REST API that is used by the Docker client (the docker command).
