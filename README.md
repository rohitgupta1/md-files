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


Although we apply LEAN to many of our projects, we decided on not to submit a MVP but a fully function website instead. Upon completion of vision statement, we discussed the high level architecture, team composition, user roles and personas, product scope and key features, and decided on various scrum ceremonies.  The next section summarizes the remainder of our kick-off meeting.

Project leader (Product Owner) – Rohit G.
Scrum master – Jim T.
Backend developer – Risa O.
Front end – Stephanie S.
UX – Hoa P.
Web design – David N.
DevOps – Jay M.
Users roles: public users, doctors, pharmacists, attorneys, FDA experts, Fed. Watchdogs
Scrum ceremonies: daily standups at 10:30am, 2-day sprints, sprint planning every other day, review, retro, and release planning to occur and the end of each sprint, entire team to attend all meetings. 
Tools: Slack.com was selected for chatting, Taiga.io for Agile project management, and GitHub for code versioning.
Initial technology stack: See final here 
frontend:
highcharts.js
bootstrap
jquery

backend:
python 2.7
postgres
memcached

Environments: We ended up selecting PWS as the test environment and AWS as our prod environment - developers to code on their local machines (Ubuntu/Macs).

In most of our current client projects, we follow an integrated ‘User-Centered Design’ processes in which we strongly encourage end-users to influence how the final design takes shape. For the FDA project, we decided on the following techniques (mainly due to time constrains).


* **Project Vision** - 
Our prototype is a Minimum Viable Product (MVP) that will meet those needs and ... [see the rest of the Project Vision](https://github.com/devis/18FAgileBPA/wiki/Project-Charter#vision)
* **Project Roadmap** - By the submission date, we will develop a Minimum Viable Product (MVP) with a basic feature set for an individual user: Produce data for two public API endpoints that ... [see the rest of the Project Roadmap](https://github.com/devis/18FAgileBPA/wiki/Project-Road-Map)
* **Prototype**: [https://devis18f.herokuapp.com](https://devis18f.herokuapp.com) continuously deployed on [Heroku IaaS](https://www.heroku.com)
* **Our Approach** - Read about the [approach](#approach) we used to develop this MVP prototype

## Contributing

Please use the [fork and pull](https://help.github.com/articles/using-pull-requests#fork--pull) collaborative model, basing your pull requests on the `master` branch.

### Prerequisites for Development Environment

Make sure you have [node.js](https://nodejs.org) installed (currently, version 0.12.4), and you can use the `npm` command:

```shell
$ npm version
```

Install [Grunt](http://gruntjs.com), our chosen build task runner, globally:

```shell
$ npm install -g grunt-cli
```

### Running Locally

Clone this repository

```shell
$ git clone https://github.com/devis/18FAgileBPA.git
$ cd 18FAgileBPA
```

Then install dependencies from the project root directory:

```shell
$ npm install
```

Start the server with a grunt task:

```shell
$ grunt serve
```

You can now open [http://localhost:8000](http://localhost:8000) in your browser.

### Testing

#### Unit tests

To run the unit tests, use the grunt task:
```shell
$ grunt test
```

There are two sets of tests that are run, one using [mocha](http://mochajs.org/) and [must](https://github.com/moll/js-must) for the backend, and one using [karma](http://karma-runner.github.io/) and [jasmine](http://jasmine.github.io/) for the frontend. When complete, you will see the results of both sets of tests (pass/fail) as well as text summaries of the code coverage, as instrumented by [istanbul](http://istanbul-js.org/), assuming there are no test failures.

You can view the full details of this coverage in a drill-down enabled report by opening:

 - Backend report: `coverage/lcov-report/index.html`
 - Frontend report: `coverage/html-report/index.html`

## Deploying

The steps defined here describe a mostly manual deployment process. This process can be automated with the use of continuous integration systems, like [Circle CI](https://circleci.com/) or [Jenkins](https://jenkins-ci.org/), and other configuration management tools, such as [Puppet](https://puppetlabs.com/) or [Chef](https://www.chef.io/).

### Using Heroku

If you would like to use [Heroku](https://heroku.com) like we have, you can follow our [Heroku deployment guide](HEROKU_DEPLOYMENT.md).

### Your own server

If you use [Docker](https://www.docker.com/) for virtualization, we have developed a [Docker container](https://github.com/devis/18FAgileBPA-docker) for your convenience.

You can also follow our [manual deployment guide](MANUAL_DEPLOYMENT.md), which provides general recommendations on installing and running the software on your own system.

## Approach

_See our [Approach Criteria Evidence](APPROACH_EVIDENCE.md)_

###Initial status
* Received notice of openFDA data source
* Stakeholders
  * Appointed internal staff as proxy users
  * Proxy users conducted brainstorming sessions to identify a problem we could solve using openFDA data
* Now with a problem defined, and a client to work for, we began our normal process, modified somewhat given the compressed timeframe and unusual circumstances.

### Project Initiation / Communication Plan
* Identify roles
* Name a Product Owner
* Create Project Plan and Schedule
* Specify Communications Plan
  * Set up chat room
  * Set scrum time
  * Set up code repository, issue tracker, project wiki
* Conduct project kickoff meeting with the client (in this case our proxy users)
* Create Risk Management plan, to be updated
  * during and after requirements elicitation with the customer
  * during release and iteration planning meetings
  * during retrospectives

### Initial Requirements Elicitation and Design Session
* Craft a [vision](https://github.com/devis/18FAgileBPA/wiki/Project-Charter#vision) for the project with users
* Conduct requirements workshop
* Produce draft user stories (no acceptance criteria yet)
* Initial prioritization of features/stories
* Enter draft users stories directly as Github issues, with a 'user-story' label

### Technical Approach
With vision and high-level user stories completed, design software infrastructure best suited to solving this problem.

#### Configuration Management
- [Grunt](http://gruntjs.com)
 - Provides scripted builds
- [npm](https://www.npmjs.com)
 - Handles automated dependency management
- [Docker](http://docker.com)
 - Provides portable containers of pre-configured software

##### Back-end / API stack
- [node.js](https://nodejs.org/)
 - JavaScript on the server
- [Express](http://expressjs.com/)
 - Minimilist web application framework
- [KrakenJS](http://krakenjs.com/)
 - Security and templating for Express applications

##### Front-end / UI tools
- [AngularJS](https://angularjs.org/)
 - Single Page Application (SPA) framework
- [Browserify](http://browserify.org/)
 - Isomorphic JavaScript framework
- [Skeleton](http://getskeleton.com/)
 - Lightweight style guide and CSS library

#### Continuous Integration
- [Circle CI](https://circleci.com/)

#### Application Monitoring
- [Data Dog](http://www.datadoghq.com/)
 - See our [public metrics](https://p.datadoghq.com/sb/zraJRV-89b5c7fe6a)

#### Code Quality monitoring
- [Code Climate](https://codeclimate.com)

#### Continuous Deployment
- [Circle CI](https://circleci.com/)
- [Heroku](https://heroku.com)

### Design Session: Complete/Prioritize User Stories
* for each story, lead a discussion between developers and users
  * add acceptance criteria to users stories
  * update stories or add new ones as required
* prioritize stories according to business value, as determined by users

### Release Planning/Iteration Planning
With user stories completed and prioritized, conduct initial release planning meeting:
* Add estimates to each story
* Group the stories into multiple releases, based on users priorities and developer time estimates
* Break user stories into tasks
* Assign stories to developers for the first iteration
* Publish a project [Project Road Map](https://github.com/devis/18FAgileBPA/wiki/Project-Road-Map) with our initial release specified as our minimum viable product (MVP).

## Daily Scrum
Start iterative development process. Given the compressed time frame:
* Use continuous deployment so the latest code would always be on the prototype server, so planning specific releases became less important
* Use a more flexible iteration process: First iteration would include user stories for an MVP.
  * took responsibility for producing an MVP by the submission date.
  * subsequent iterations could be planned during daily scrums to add additional features from our release plan and road map

## Acceptance Testing
* Using continuous deployment allowed continuous testing
* Product Owner performed acceptance testing as builds were deployed, incorporating additional testing feedback from users
  * Throughout testing, new issues or defects were recorded, and new user stories added to the backlog
  * Product Owner closed user stories as acceptance criteria were met
