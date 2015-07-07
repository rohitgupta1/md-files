# Artemis Consulting's response to GSA 18F's Agile Delivery Services  RFQ993471

## Key Metrics

[![Sprints](https://github.com/taigaio)](6)
[![User Stories Completed](https://github.com/taigaio)](40)
[![User Interviews conducted](https://...)](2)
[![Test Coverage](Django unit tests)](96%)

## Background

Lorem ipsum

## Project Kick Off

Artemis Consulting kicked off this agile project nicknamed "FDA Drug Monitor" by assembling the project team and discussing the 18F opportunity/problem statement. This statement describes the current business’s situation that creates the need for this project. We decided on the following statement: “We should be able to produce a usable, mobile-friendly and accessible public website using OpenFDA's APIs for drugs, and win one of the BPAs in the process”. 
Next, we created a concise vision statement to ensure that the solution actually meets the intended product owner and users’ goals.  This shared Vision Statement helped to keep our team focused: "To deliver a fast, responsive and intuitive API-driven website using the Drug Labels API, Adverse Events API and Enforcement Actions API that brings information together for the public and other potential users in a holistic fashion, within the next 6 days".  

## Kickoff
Although we apply LEAN to many of our projects, we decided not to submit a MVP but a fully functional website instead. Upon completion of vision statement, we discussed the high level architecture, team composition, user roles and personas, product scope and key features, and decided on various scrum ceremonies.  The next section summarizes the remainder of our kick-off meeting.

## Project Scope
Since the original RFP had a due date of xx/xx/15, the team had to place boundaries around the solution by deciding which features and system functions to focus on. Due to time constraints, the decision was made de-scope all ‘food’ elements from our system and revisit this subject area during later releases. Off-line browsing (e.g. keep the service in case the FDA APIs are down) was another key feature the team decided to de-scope. Defining the project scope early on helped the team set stakeholders’ expectations while providing sufficient details and features for the team to focus. 
•	Use the following format – they should be short (to be completed):
•	<<Production scheduling>>
•	<<Management reporting>>
•	Browse drugs by label
•	Search drugs by label
•	Browse adverse reactions by frequency
•	Search adverse reactions
•	Browse drug enforcement actions by state
•	Browse adverse reactions by gender
•	Submit questions using a “Contact Us” form

In order to deliver these system features, the team decided to use and remix these APIs for the project:
1.	Drug Labels API
2.	Adverse Reaction API
3.	Enforcement Action API

#### Team roles

Project leader (Product Owner) – Rohit G.
Scrum master – Jim T.
Backend developer – Risa O.
Front end – Stephanie S.
UX – Hoa P.
Web design – David N.
DevOps – Jay M.

The project team (and stakeholders) decided on ‘promoting’ Rohit as the project leader based on his qualifications and the technical product manager (TPM) role he performs on the Congress.gov contract. Rohit will be held responsible for how well the service will meet the needs of its prospective users, ensuring that features as part of the project scope are built, as well as managing the feature and defect backlogs on a daily basis. [Play 6 checklist](Play 5 checklist).  The team members assembled for this project are experts in their respective disciplines. Click here to view the [Play 7 checklist](Play 7 checklist).

####System user roles
Public users, doctors, pharmacists, attorneys, FDA SMEs/employees, Federal regulators, Federal Watchdog agencies, state regulators

####Scrum ceremonies
Daily standups at 10:30am, 2-day sprints, sprint planning every other day, review, retro, and release planning to occur and the end of each sprint, entire team to attend all meetings. Backlog grooming and reprioritization happened daily. To view all our agile artifacts, click on this link -> [LINK](LINK)t

####Tools 
Slack was selected for chatting and online collaboration, Taiga.io for Agile project management, and GitHub for code versioning. The modern technology stack chosen by team is all open source with hosting being the only exception. By selecting the technology stack below, the team strongly feels that it can develop and prototype effectively while delivering a product that is cost-effective and can scale easily. [Play 8](Play 8) 

## Initial technology stack: See See final [frontend tech stack here](frontend tech stack) and the [backend stack here](backend tech stack) 
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

#### Configuration Management
- [Docker](http://docker.com)
 - Provides portable containers of pre-configured software

#### Testing
Selenium
pyunit testing framework

#### Environments 
We used Pivotal Web Services CloudFoundry as the development/test environment and Amazon Web Services as our production environment. Developers coded on their local machines (running Ubuntu/MacOS) to code the prototype.

#### Continuous Integration
- [Jenkins](http://jenkins-ci.org/)

#### Application Monitoring
- [Nagios](https://www.nagios.org/)

#### Continuous Deployment
- [Jenkins](http://jenkins-ci.org/)
- [Pivotal CloudFoundry](http://pivotal.io/platform-as-a-service/pivotal-cloud-foundry)

In most of our current client projects, we follow an integrated ‘User-Centered Design’ processes in which we strongly encourage end-users to shape how the final system gets developed. For the FDA project, we decided on the following UCD techniques (mainly due to time constraints): user personas, user journeys, usability testing, interviews, expert reviews, and prototypes.  

Developing user personas and journeys early on the design process helps the team to ‘understand’ what prospective users of the system really want.  These initial user exploration sessions also help us better create more realistic and better ‘user’ stories overall.  Success of a design team is often measured by the amount of information they have about prospective users. Conducting interviews is a quick but excellent method of discovering facts, opinions, and behaviors held by potential users.  The analyzed results of these interviews tend to complement other UCD techniques. In our case, they directly feed into the user personas and journeys to add depth thus, making them more realistic and complete.   See final interview questions here -> [Link](Link)

Based on the analyzed interview results, the team ended up with the following personas:

Novice – public users, concerned parents, students, people in the drug and food industry
Professional – doctors, pharmacists, mainly medical professionals
Specialist – Attorney, policy makers, and maybe bloggers
Experts – FDA employees, state regulators, federal watchdogs

Click on the links to see the [final user personas](http://....) and [final user journeys](http://....)


Developing User journeys is an excellent user-centered design technique to follow prospective users from start to finish.  However, addressing the whole (user) experience, and how they interact with the system on the go or by mobile devices, requires the gathering of additional metrics and usability testing of our prototypes.  Some of the user pain points the team discussed and will trytried to mitigate as part of the design include: accessibility, 508 compliance, browser compatibility, etc << insert more here >>.  The team strongly felt that applying the UCD techniques in the sections previously mentioned satisfy Play [1] and [2]. 

When teams have accurate user data at their disposal, the task of designing simple, intuitive, easy-to-use but powerful, interface becomes much more straight-forward.  The key here was making the service user friendly instead of frustrating or confusing.  Due to time constrains, the team decided against creating a (more traditional) style guide from scratch but opted to use Bootswatch Paper theme as the design style guide and pattern library for the website. By using this flexible style guide for design and incorporating accessibility best practices, the team felt confident that they have satisfy Play 3, ensuring all prospective users can navigate the service intuitively and can obtain the information they want from the service, in a easy and consistent way. [Play 3](http://...)

Artemis Consulting uses gile scrum for all their internal development efforts and for most of our client projects. For most of our projects, sprints are usually 1-2 week in duration but never exceed 3 weeks. In general, the shorter the sprints, the faster feedback we receive from our users and clients. This feedback enables the team quickly make the necessary adjustments, avoiding potential long-term and costly rework. 

Although the team is experienced with Jira Agile and Pivotal Tracker, the decision was make to go with Taiga for agile project management and defect tracking. Taiga tends to be more ‘lightweight’ for project with relative quick turnarounds and firm deadlines. 

All our agile artifacts our related to Play 4, can be found [here](http://...). Results of usability testing can be viewed [here](http://...)
For automated testing, we used [Selenium](http://...). The scripts for these tests are checked in [here](http://...) 


## Flexible hosting environment 

During Sprint 0, the team performed various user analysis tasks and worked on deploying the hosting environment for both test and production. For the test environment (including continuous integration and continuous deployment), the team picked Pivotal's CloudFoundry service(a.k.a. PWS), and for production, the team chose Amazon Web Services (AWS). Both are flexible infrastructures, where additional resources can be provisioned in real-time to meet user demand. For the prototype’s testing environment, the team decided on using Pivotal Web Services (PWS) CloudFoundry, an open (and agile) platform as a service (PaaS).  The Cloud Foundry platform required minimal setup while still proving rapid deployment and scaling capabilities.  Jenkins on CloudBees was utilized for continuous integration and deployment integrated with Github. A Jenkins job periodically runs unit tests, and if the tests are successful, deploys the latest code from the repository to the CI/CD environment. If the tests are unsuccessful, an email is sent out to the appropriate developer. 

For production, the team felt that Amazon Web Services was the better choice because AWS has been around for almost a decade now and offers highly reliable, scalable, and relatively inexpensive cloud hosting services.  The AWS management console is simple and relative straightforward web-based tool. Another driver for using AWS is the government’s interest in migrating parts of their IT infrastructure into the AWS GovCloud. AWS was officially approved for government use in 2013 and their regions and availability zones are geographically the most dispersed and redundant cloud services available.  [Pool 3 requirements D, Play 9](http://....)


#### Prototype
[http://opendatafda-artemis-staging.cfapps.io or http://demo.artemisconsultinginc.com](http://opendatafda-artemis-staging.cfapps.io) continuously deployed on [Pivotal CloudFoundry](http://pivotal.io/platform-as-a-service/pivotal-cloud-foundry)


## Continuous Monitoring

Using AWS for the production environment also provides additional integration benefits – such as Continuous Monitoring (CM).  For this prototype, we installed CloudWatch and Threat Stack, two monitoring services that are built for AWS.  CloudWatch provides basic and detailed monitoring services and can monitor resource utilization, application and database performance, log files, and overall system’s health. If time permits, we will try to monitor custom metrics of the prototype via a simple API. The service provides a dashboard with graphs, statistics, and alarms. 

Threat Stack is a Continuous Security Monitoring service for (AWS) cloud.  Threat Stack was built to help AWS users protecting their cloud instances from intrusions and data loss by continuously monitoring and providing insights into their systems.  Unlike most intrusion detection software platforms that are difficult to install and requires expertise to use, Threat Stack’s simple interface is intuitive and the tool can be configured in minutes. Threat Stack provides users with a REST API that savvy developers can use to obtain real-time information about agents, alerts, and policies.  [Pool 3 requirements F, Play 9](http://...)


## Configuration Management  
The team decided to use Puppet for automated configuration management.
[Docker](https://www.docker.com/) is used for container virtualization, a Docker container is available at .. ..................

[Pool 3 requirements G](http://...)


## Automated testing and deployments
Unit testing reduces the amount of bugs get into the code and potentially, into production.  Since automated tests can be ran as frequently as needed, and the use of automated test suites makes it easier to change and refactor code later on, unit testing saves precious development time during the life cycle of the product.  For this prototype, the team built a suite of automated tests, which tested the app as well as ensured wide code coverage (>95%). The Pyunit framework was used for unit testing. The team selected Selenium WebDriver for automated web testing. Jenkins was used as our continuous integration and continuous deployment tool.  Upon code commits/checkins into GitHub, Jenkins automatically runs the unit test suites. If the unit tests pass, the code is automatically promoted to the testing/integration environment.  To view the Selenium testing scripts, click [here](http://....). The coverage is currently at >95%.  [Pool 3 requirements F, Play 10]

#### Prerequisites for Development Environment

Install the following for system level dependencies for Ubuntu
```shell
$ sudo apt-get install python python-dev apache2 libapache2-mod-wsgi git python_psycopg2 libpq-dev memcached
```

Clone this repository into desired $APP_DIR
```shell
$ git clone https://github.com/artemis-consulting/prototype-pool3 $APP_DIR
$ cd $APP_DIR/code
```
Create the database:
```shell
sudo su - postgres
createdb prototype
createuser -P proto_user
```
choose 'proto_pass' as password.  If choosing a different password, keep it handy to modify in the settings file later.
```shell
psql
```
Grant privileges to the user
```shell
# GRANT ALL PRIVILEGES ON DATABASE prototype TO proto_user;
```
Create a virtualenv
```shell
virtualenv aretmisprototype
source $APP_DIR/artemisprototype/bin/activate
```
Install the Python modules using pip. 
```shell
pip install -r code/requirements.txt
```

Run django commands
```shell
python manage.py migrate
python manage.py collectstatic
```

Make changes to the settings file if needed.
Change DATABASE settings if you changed the password for example
Change ALLOWED_HOSTS to appropriate domain name if you're not using localhost


### Running Locally
To test the install, use django's runserver command
```shell
python manage.py runserver
```
You can now open [http://localhost:8000](http://localhost:8000) in your browser.
Set up Apache using mod_wsgi
https://code.djangoproject.com/wiki/django_apache_and_mod_wsgi

Sample apache config for django running daemon mode with virtualenv:
```shell
<VirtualHost *:80>

 WSGIDaemonProcess prototype python-path=/apps/prototype/code:/apps/env/lib/python2.7/site-packages
 WSGIScriptAlias / /apps/prototype/code/opendata_fda/wsgi.py process-group=prototype

 Alias /static/ /apps/prototype/code/.static/
 
 <Directory /apps/prototype/code/opendata_fda>
 Require all granted
 </Directory>
 
 <Directory /apps/prototype/code/.static>
 Require all granted
 </Directory>
 
</VirtualHost>
```

Start Apache


You can now open [http://localhost:80](http://localhost:80) in your browser.

### Testing

#### Unit tests

To run the unit tests, use django's test framework with coverage
```shell
$ python manage.py test core --with-coverage --cover-html --cover-package=core
```
The unit tests will also kick off the selenium tests.
You can view the full details of coverage in a drill-down enabled report by opening:

 - Backend report: $APP_DIR/cover/index.html

## Deploying

As mentioned earler, the deployment process can be automated with the use of continuous integration systems, like [Jenkins](https://jenkins-ci.org/), a cloud-based Jenkins installation like [CloudBees](https://www.cloudbees.com/), and other configuration management tools, such as [Puppet](https://puppetlabs.com/) or [Chef](https://www.chef.io/).

### Docker image

If you use [Docker](https://www.docker.com/) for virtualization, a Docker container is available at .. ..................

## Approach

_See our [Approach Criteria Evidence](APPROACH.md)_
