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