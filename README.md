# Artemis Consulting's response to GSA 18F's Agile Delivery Services  RFQ993471

## Key Metrics

[![Sprints](https://github.com/taigaio)](6)
[![User Stories Completed](https://github.com/taigaio)](40)
[![User Interviews conducted](https://...)](2)
[![Test Coverage](Django unit tests)](96%)

## Background

Lorem ipsum

## Project Kick Off

Artemis Consulting kicked off this “PROJECT_NAME” in agile fashion by assembling the project team and discussing the 18F opportunity/problem statement. This statement describes the current business’s situation that creates the need for this project. We decided on the following statement: “We should be able to produce a FDA API product better, faster, (and cheaper), than our competitors – and win one of the BPAs in the process”. 
Next, we created a concise vision statement to ensure that the solution actually meets the intended product owner and users’ goals.  A shared Vision Statement among all team members helps ensure that the solution meets the intended goals while keeping the team laser focused. Below is our project vision.
“To deliver the highest quality and most elegant API driven website for the public audiences within the next 6 days”.  

## Kickoff
Although we apply LEAN to many of our projects, we decided not to submit a MVP but a fully functional website instead. Upon completion of vision statement, we discussed the high level architecture, team composition, user roles and personas, product scope and key features, and decided on various scrum ceremonies.  The next section summarizes the remainder of our kick-off meeting.

####Team roles

Project leader (Product Owner) – Rohit G.
Scrum master – Jim T.
Backend developer – Risa O.
Front end – Stephanie S.
UX – Hoa P.
Web design – David N.
DevOps – Jay M.

####User roles
Public users, doctors, pharmacists, attorneys, FDA experts, Federal Watchdogs agencies, state regulators

####Scrum ceremonies
Daily standups at 10:30am, 2-day sprints, sprint planning every other day, review, retro, and release planning to occur and the end of each sprint, entire team to attend all meetings. 

#### Configuration Management
- [Docker](http://docker.com)
 - Provides portable containers of pre-configured software

####Tools 
Slack was selected for chatting and online collaboration, Taiga.io for Agile project management, and GitHub for code versioning.

## Initial technology stack: See final[Final stack] here 
#### Front-end development
Django templates 1.8.2
JavasScript/jQuery
Bootstrap/Bootswatch Paper theme
Highcharts chart and mapping widgets
(Proprietary) accessibility toolkit

#### Back-end development
Apache 2.4.7
Python 2.7.10
Django 1.8.2
Memcached 1.4.27 
Postgres 9.4

#### Testing
Selenium
pyunit testing framework

#### Environments 
We used Pivotal Web Services CloudFoundry as the development/test environment and Amazon Web Services as our production environment. Developers coded on their local machines (running Ubuntu/MacOS).

#### Continuous Integration
- [Jenkins](http://jenkins-ci.org/)

#### Application Monitoring
- [Nagios](https://www.nagios.org/)

#### Continuous Deployment
- [Jenkins](http://jenkins-ci.org/)
- [Pivotal CloudFoundry](http://pivotal.io/platform-as-a-service/pivotal-cloud-foundry)

In most of our current client projects, we follow an integrated ‘User-Centered Design’ processes in which we strongly encourage end-users to influence how the final design takes shape. For the FDA project, we decided on the following techniques (mainly due to time constrains).

## Our Approach - Read about the [approach] Artemis used to develop this prototype

## Prototype
[http://opendatafda-artemis-staging.cfapps.io or http://demo.artemisconsultinginc.com](http://opendatafda-artemis-staging.cfapps.io) continuously deployed on [Pivotal CloudFoundry](http://pivotal.io/platform-as-a-service/pivotal-cloud-foundry)

#### Prerequisites for Development Environment

Install the versions listed above for Python, Django, Less, Memcached and Postgresql. 
```shell
$ sudo apt-get install python
$ sudo apt-get install django
$ sudo apt-get install less
$ sudo apt-get install memcached
$ sudo apt-get install postgresql
```

Install the following Python modules using pip. 


apt-xapian-index (0.45)
chardet (2.0.1)
Cheetah (2.4.4)
cloud-init (0.7.5)
colorama (0.2.5)
configobj (4.7.2)
dj-database-url (0.3.0)
Django (1.8.2)
django-nose (1.4)
django-rednoise (1.0.5)
gunicorn (19.3.0)
html5lib (0.999)
jsonpatch (1.3)
jsonpointer (1.0)
Landscape-Client (14.12)
mock (1.0.1)
nose (1.3.7)
oauth (1.0.1)
PAM (0.4.2)
pip (7.1.0)
prettytable (0.7.2)
pycurl (7.19.3)
pyOpenSSL (0.13)
pyserial (2.6)
python-apt (0.9.3.5ubuntu1)
python-debian (0.1.21-nmu2ubuntu2)
python-memcached (1.54)
PyYAML (3.10)
requests (2.7.0)
selenium (2.44.0)
setuptools (3.3)
six (1.5.2)
ssh-import-id (3.21)
Twisted-Core (13.2.0)
Twisted-Names (13.2.0)
Twisted-Web (13.2.0)
urllib3 (1.7.1)
virtualenv (1.11.4)
wheel (0.24.0)
whitenoise (2.0)
zope.interface (4.0.5)

The requirements.text file that is part of the "code" directory can be sent to pip. 
```shell
 pip install -r code/requirements.txt
```

### Running Locally

Clone this repository

```shell
$ git clone https://github.com/artemis-consulting/prototype-pool3
$ cd code
```

Set up Apache using mod_wsgi
https://code.djangoproject.com/wiki/django_apache_and_mod_wsgi

Start Apache


You can now open [http://localhost:80](http://localhost:80) in your browser.

### Testing

#### Unit tests

To run the unit tests, use the pyunit task:
```shell
$ 
```
You can view the full details of coverage in a drill-down enabled report by opening:

 - Backend report: `...`
 - Frontend report: `..`

## Deploying

The steps defined here describe a mostly manual deployment process. This process can be automated with the use of continuous integration systems, like [Jenkins](https://jenkins-ci.org/), a cloud-based Jenkins installtion like [CloudBees](https://www.cloudbees.com/), and other configuration management tools, such as [Puppet](https://puppetlabs.com/) or [Chef](https://www.chef.io/).

### Docker image

If you use [Docker](https://www.docker.com/) for virtualization, a Docker container is available at .. ..................

## Approach

_See our [Approach Criteria Evidence](APPROACH.md)_
