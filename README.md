# Python Applications - Practices to follow

## Choosing a web framework for application 
Python apps will need a web framework either there are some screens or some rest endpoints. There are full-stack and non full-stack (micro frameworks) frameworks in python. Depending on the usecase we can select the framework, lighter the better. 
https://wiki.python.org/moin/WebFrameworks
Consider the features your application will need , evaluate and compare what the framework provides, before making the call. It is not necessary to go for a full-stack framework when we need a sercure Rest based service since it has pre-built security, we can add some extra security in microframework as well.
https://www.fullstackpython.com/web-application-security.html
https://pythonhosted.org/Flask-Security/
## Package your application / project
It is easy to package the python project for distribution. If we choose to distribute within a closed group, then we can upload to a remote private repository and install it from there also. Here are some useful links.
https://packaging.python.org/tutorials/packaging-projects/
https://docs.djangoproject.com/en/2.2/intro/reusable-apps/#id1
https://setuptools.readthedocs.io/en/latest/https://www.digitalocean.com/community/tutorials/how-to-package-and-distribute-python-applications

## Documentation
Add line comments and block comments whereever you can. Adapt to any documentation editor plug-in. Make sure all the team members has similar one to do the same. If you think any of your code or block of code needs / will need explanation for an other guy to understand, add a line comment.
extensions like docBlocker is easy to add structured documentation.
## Readability

## Naming Convensions
Try to follow the same naming convension among the project team. Try to include as much information about a variable or function in its name, in minimum possible length. 
https://visualgit.readthedocs.io/en/latest/pages/naming_convention.html

## Packing Requirements
Find and use only the packages that should be in requirements for a project. Use pipdeptree, pip_check_reqs freequently to manage the requirements file. Keep it clean as far as possible. It's better to add a test or a commit hook which will check for the missing dependancy or unwanted dependancy in requirements.

## Folder Structure
Divide the functionalities carefully into modules. src folder is not necessary.
## Versioning

## Git Commit Hooks
There is a `hooks` folder inside the `.git` folder in our git project. Which will have a number of scripts, each will be executed just before we carry out the git action `commit`,`push`, `rebase` etc. We can define some actions like validation in each script.
### Pre-Commit
#### Automatic Code Formatting 
#### Linting
Linting can either be done from within the pre-commit, or with  pylint (http://pylint.pycqa.org/) or even from the ide or code editor. Don't use all three , choose the best which always works and ignore the rest, so that there are no conflicts amoung them.
## TDD - Test Driven Development

## Unit Testing
### Tests in python packages
Use tools like tox to check whether 
* the package works in different python versions
* running your tests in each of the environments, configuring your test tool of choice
* acting as a frontend to Continuous Integration servers, greatly reducing boilerplate and merging CI and shell-based testing

## CI/CD
