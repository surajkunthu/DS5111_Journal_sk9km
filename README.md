# DS5111 Journal - Fall 2023
Suraj Kunthu - sk9km

# Module 01: Git Fundamentals, Setting up github repository and AWS login

I’m excited to learn more about Data Engineering and the back end! Fortunately, I’m coming in with some experience with Git and GitHub so reading the text was more of a refresher than anything else. I’ve never touched any AWS services so it’s exciting to be able to experiment within an instance. I thought learning about makefile’s was interesting. I knew shell scripts (.sh) were used for automation purposes but never heard of makefiles.

# Module 02: Software Skills I
It’s nice to refresh my knowledge on modules and packaging python files for applications. In the MSDS program, I’ve only ever done it for one project and always wanted to tackle something like that again. 

I’ve never heard of Tmux before but after reading more I’m eager to try it out. However, I still do not see its usefulness as of right now. I can open multiple instances of my current terminal and it seems that it serves the same purpose. Unless there is more to Tmux than meets the eye? Maybe it is a better way to “monitor” terminal instances and keep track of kernel command history?

# Module 03: Software Skills II

It was useful to learn more about decorators in Python. I've heard about them before but never used them. I can definitely see how they would be useful as it provides a better way to chain functions together for modifying an object's structure. The Python decorator provides a cleaner way for this implementation that would help reduce redundancy and make code DRY with the `@` symbol:

```python
@testfunction1
def test:
    print("hi")
```

# Module 04: Software Skills III

I have heard of virtual environments before but never personally used them. I have seen online that virtual environments make, and in some of the classes in the MSDS program, that creating virtual environments will make managing packages and dependencies a lot easier. However, I did not experiment with it until now within my AWS EC2 instance. I finally understand why creating a virtual environment is very useful. I can now "hand-off" my code to someone else and, with a makefile that contains specific commands and requirements, they can reproduce my results without any versioning issues.

During the lab I learned that once you create the virtual environment with:

```bash
python3 -m venv name_of_environment
```

You have to `activate` the environment with:

```bash
. name_of_environment/bin/activate
```

# Module 05: Software Testing

I have dealt with Software Testing before and I believe it is an extremely valuable part of software development. In the MSDS program, we've only written unit tests for our final project in DS 5100 with `pytest`. In my day job, my team primarily writes code in TypeScript/JavaScript and we utilize `Jest.js` to write our test suites.

# Module 06: CICD

Much like the software testing module, I believe anything that can automate software testing and determine it's integrity will make for better code and cohesiveness within teams. Since, Agile is the primary project management methodology leveraged, CI/CD tools make it much easier to provide reliable code for your team and/or your client(s). GitHub actions and workflows is just another example of this "pipeline" that helps automate deployment.

# Module 07: Containers

Docker is an amazing tool that further helps eliminate that age-old issue of "it works on my pc" when handing-off your code to someone else. Creating a container ensures that everything down to the OS is the same between test runs of the code because of the image that is created with Docker. This also helps when deploying updated versions of code since now it makes it easier to isolate what could be a potential issue when upgrading. If an issue does arise, it is very simple to rollback to the previous image.

# Module 08: Database Design

Databases are an important concept, not just for Data Science, but for the greater software engineering community. Everything relies on data. Whether it be from an API or database server, proper design is required to make these "transactions" as simple as possible. Luckily, the data community has standarized many aspects of data retrieval and formatting. One such is the creation of CRUD and CRUD properties. These properties (Create, Read, Update, Delete) MUST exist to interact with one's database. This in combination with a relational database allows for any developer/engineer approaching this database/API the groundwork to leverage the data within without any hurdles.

# Module 09: Data Build Tool (DBT)

DBT is a useful framework to help modularize SQL and creating Databases. As a full-time software engineer, having to create relational databases can be tedious especially if you need to add a new field to a datatable. Although NoSQL databases can solve some of these problems, NoSQL databases are not always the ideal tool to use. A DBT can be used to mitigate that gap of creating a new database, updating it with new requirements, and provide some basic data testing.

# Module 10: Snowflake

Snowflake seems to be a great enterprise tool that allows multiple groups of people to access the same data with different layers of privilege. This is an excellent way of perserving data security as groups that do not need write/delete access will not accidentally destroy any data. While those with that access can focus on maintaining the databases and build new tables. It was pretty effortless to use dbt to build SQL tables and connect it to Snowflake.

