# Intra V2 API
Main source of documentation: https://api.intra.42.fr/apidoc

## Overview
Below is a list of endpoints available in the Intra v2 API, which is used to access various resources and data related to the 42 Network. Each endpoint includes a brief description and example usages.

### Accreditations
TODO

### Achievements
Intra achievements
- Find out which achievements are available for a cursus or campus.

### Achievements Users
Link between users and achievements.
- Find out which users have which achievements and when they were unlocked.

### Amendments
TODO (Something about internships)

### Announcements
Announcements are shown to users on the Intra dashboard as banners. They are not intended to be used lightly.
- Find out which announcements are currently active for which campus.

### Anti-grav Units
TODO

### Anti-grav Units Users
Postponements of the deadlines for users **in the Black Hole System**.
- Find out which users have postponed their deadlines, when they were postponed, and calculate what the new deadlines are for them.

### Apps
Apps are used to access the Intra v2 API. Both students and staff can register apps.
- Find out which apps are registered and by whom
- List the roles of the apps (defines the permissions of the app)
- Get meta information about the app, such as its name, a description, the website and image.

### Attachments
Attachments are files that can be attached to Intra projects. They used to also be used for forum related things, but that is no longer the case.
- Find out which attachments are available for a given project.

### Balances
TODO (Something about evaluation point donation pools)

### Bloc Deadlines
The start and end dates of coalition tournaments.
- Find out when the next coalition tournament starts and ends.

### Blocs
Contains the definitions and configurations of coalitions for a cursus at a campus.
- Get the list of coalitions for a cursus at a campus.

### Broadcasts
TODO

### Campus
Definitions of campuses within the 42 Network.
- Find out which campuses exist
- Get the amount of users in a campus
- Get the physical location of a campus
- Get the website and social media links of a campus

### Campus Users
Link between users and campuses.
- Find out which users are in which campus and when they joined.
- Figure out which campus is a user's primary campus (where they are currently studying).

### Certificates
TODO

### Certificates Users
TODO

### Closes
An active close prevents users from accessing the Intra.
- Find out which users have dropped out and when
- Find out which users are currently prohibited from accessing the Intra
- Find out which students have (had) community service obligations
- Find out the reason why a student stopped studying at 42 Network

### Clusters
Defines a cluster (a group of computers) at a campus. Not often used.
- Find out which clusters exist at a campus

### Coalitions
Holds information about each coalition, such as its name, emblem, color and score.
> You might want to take a look at the [Blocs](#blocs) endpoint instead, or even the [Blocs Deadlines](#bloc-deadlines) endpoint.
- Find out the current score of a coalition
- Find out the name, emblem and color of a coalition
- Find out the leader of a coalition

### Coalitions Users
Link between users and coalitions.
- Find out which users are in which coalition and when they joined

### Commands
TODO (Something about the Intra shop)

### Community Services
A community service is a task that a user must complete as a punishment for a rule violation.
> Usually you'll want to look at the [Closes](#closes) endpoint instead.
- Find out what obligation a user's close has, if any

### Companies
TODO

### Correction point historics
TODO

### Cursus
A cursus is a curriculum that a user can follow at a campus. Each project and exam belongs to a cursus.
- Find out which cursuses exist and what their names are

### Cursus Users
Link between users and cursuses.
- Find out which users are in which cursus
- Find out when a user started and ended a cursus
- Find out if a user has a coalition for said cursus
- Get the grade and level of a user in a cursus

### Dashes
TODO

### Dashes Users
Link between users and dashes.

### Endpoints
Defines the link between the Intranet and the Campus IT infrastructure. Sort of like webhooks, but more closed off. Used for things like user creation, user deletion, and user updates, including password changes.
- Find out which endpoints are available for a given campus

### Evaluations
> You're probably looking for the [Scale Teams](#scale-teams) endpoint instead.

### Events
Calendar events that are available for a campus and/or cursus.
- Find out which events are available for a campus and/or cursus and when they start and end
- Get the maximum number of participants for an event
- Get the current amount of registered participants for an event
- Find out where a given event is located
- Get the themes an event has, if any
- Get the maximum date of unregistration for an event

### Events Users
Link between users and events.
- Find out which users are registered for which events and when they registered

### Exams
Like events, but for exams.
- Find out which exams are available for a campus and/or cursus and when they start and end
- Get the maximum number of participants for an exam
- Get the current amount of registered participants for an exam
- Find out where a given exam is located
- Get the IP ranges of computers allowed to access the exam
- Get a list of exam projects that can be completed during the exam
- Figure out which cursuses an exam belongs to

### Exams Users
Link between users and exams.
- Find out which users are registered for which exams and when they registered

### Experiences
TODO

### Expertises
User defined skills that can be used to find users with specific skills.
- Find out which expertises are available

### Expertises Users
Link between users and expertises.
- Find out which users have which expertises and when they were added
- Find out how much experience a user has stated to have in a given expertise

### Feedbacks
Get the feedbacks that users have given to an evaluation or an event.
- Get the rating and comment of a user for a given evaluation or event
- Figure out when a user gave the feedback

### Flags
Flags are used at the end of an evaluation to indicate the final result of a user's project.
e.g. "OK", "Crash", "Outstanding work", etc.
- Find out which flags exist within Intra

### Flash Users
Link between users and flash messages (alert dialogs on Intra).
- Find out which users have been or will be shown which flash message
- Find out which users have seen which flash message

### Flashes
Flashes are alert messages that are shown to users on Intra.
- Get the title and content of a flash message
- Get the duration that a flash message is shown to users

### Gitlab Users
Defines public SSH keys of students that can be used to authenticate with the Vogsphere Git server at the primary campus.

### Groups
Groups are essentially used as tags/labels that are displayed on a user's profile.
- Find out which groups exist and what their names are
- Get the color of a group

### Groups Users
Link between users and groups.
- Find out which users are in which group and when they joined

### Internships
TODO

### Journals
Event log of Intra, only available to staff.

### Languages
Languages that the Intranet supports (mostly French and English).
- Find out which languages are available

### Languages Users
Link between users and languages. Not used a lot: most users use either French or English. The rest of the tranlations are not very up to date.
- Find out which users use which language on the Intranet

### Levels
TODO

### Locations
Computer logins at a campus for a single user.
> The V3 Chronos API is better suited for this purpose as it supports multiple location sources, but this endpoint is still available.
- Find out which computers a user has logged in to at a campus and when
- Find out how long a user has spent behind a computer at a campus

### Mailings
E-mails sent from within Intra to users.
- Find out which users have received which e-mails and when
- Get the subject, attachments and content of an e-mail

### Notes
TODO

### Notions
TODO

### Offers
Offers are internship offers that are available for students to apply to on the Companies page on the Intranet.

### Offers Users
TODO

### Params Project Sessions Rules
TODO

### Partnerships
TODO

### Partnerships Users
TODO

### Patronages
TODO

### Patronages Reports
TODO

### Pools
A pool is a piggy bank students can donate evaluation points to. When the pool has reached a certain amount, it will be used for evaluation point sales, which run until the pool is empty.
> Not to be confused with a Pool for a user which is when they did the Piscine.
- Find out which pools exist for which cursus and campus
- Get the amount of evaluation points in a pool
- Get the limit of evaluation points in a pool (when the pool will be used for evaluation point sales)

### Products
Products sold in the Intra shop.
- Find out which products are available in the Intra shop at which campus
- Get the price of a product
- Get the image and description of a product

### Project data
Defines the location of a project on the Holy Graph.
> Keep in mind the Common Core projects are hardcoded in the Intra, so you won't find up-to-date information about them here.
- Get the coordinates of a project on the Holy Graph
- Get the kind of project (e.g. "project", "exam", "piscine", etc.)

### Project Sessions
A project session defines a particular behaviour for a project, based on the cursus and/or the campus.
- Check if a project is intended to be alone or in a group at a campus
- Get the estimated duration of a project at a campus
- Check if a project is subscriptable or not at a campus
- Get the amount of evaluations required for a project

### Project Sessions Rules
Defines the rules for a project at a campus.
> TODO: How are these different from the [Rules](#rules) endpoint?
- Check the amount of time a user has to wait after failing a project until they can retry it
- Check the rules for finding evaluation slots for a project at a campus
- Get the passing grade for a project at a campus

### Project Sessions Skills
Defines the skills achieved by completing a project at a campus.

### Projects
Projects are the core of the Intra. They are the tasks that students must complete to progress in their cursus.
- Find out which projects are available for a cursus and/or campus
- Get the name, difficulty and description of a project
- Check if a project is an exam or a regular project
- Get subprojects of a project, if any (e.g. Internships)

### Projects Users
Link between users and projects.
- Find out which users are subscribed to which projects and when they subscribed
- Find out which users have completed a project and when they completed it
- Get the status of a project for a user (e.g. "in_progress", "finished", "failed", etc.)
- Get the final mark of a project for a user
- Check if a user has passed a project or not
- List the teams (retries) of a project for a user
- Check how often a user has retried a project (occurrences)
- Get the current team id of a project for a user

### Quests
Quests are a series of projects that a user must complete to progress in their cursus. In the Common Core, each rank has 1 linked quest.
- Find out which quests are available for a cursus and/or campus

### Quests Users
Link between users and quests.
- Find out which rank or milestone a user has completed

### Roles
Defines permissions available for apps.
- Find out which roles are available for apps.

### Roles Users
Find out which permissions an app has. Used to also be used for staff accounts, but this is no longer the case.
- Find out which apps have which permissions and when they were added

### Rules
> TODO: How are these different from the [Rules](#rules) endpoint?

### Scale Teams
Evaluations done by students for students on their projects.
- Find out how many evaluations a user has done
- Find out how many times a user has been evaluated
- Get the feedback of evaluator towards the evaluated user
- Get the final mark the evaluator has given to the evaluated user
- Find out when an evaluation was planned, when it was started and when it was finished
- Get the flag the evaluator has given to the evaluated user (e.g. "OK", "Crash", "Outstanding Project", etc.)
- Find out who evaluated whom

### Scales
The evaluation sheets used during evaluations.
- Get the questions of an evaluation sheet

### Scores
Points given to a coalition in the name of a user.
- Find out which users have given points to which coalition and when
- Find out the reason points were given

### Skills
TODO

### Slots
Slots define times a user is available to evaluate another user.
> Only staff can see who opened which slots.
- Find out when a student is or was available to evaluate another student

### Squads
Squads are groups of users that join a coalition together.

### Squads Users
Link between users and squads.
- Find out which users are in which squad and when they joined

### Subnotion
TODO

### Tags
TODO
> You might be looking for the [Groups](#groups) endpoint instead, which is used to display tags on user profiles.

### Tags Users
TODO

### Teams
Teams are groups of users that work together on a single project. A new team is created for each retry of a project.
- Find out which users are in which team and when they joined
- Find out which project a team is working on
- Get the git repository url of a team
- Get the status of a team (e.g. "searching_a_group", "in_progress", "waiting_for_correction", "finished", "failed", etc.)
- Get the final mark of a team for a project
- Check if a team has passed a project or not

### Teams Uploads
An automated evaluation done by Moulinette on a team's work.

### Teams Users
Link between users and teams.
- Find out which users are in which team and when they joined
- Find out who is the leader of a team

### Titles
Titles are a way of adding a prefix or suffix to a user's login name. They are displayed on the Intranet and are seen as a fun reward next to achievements.
They are defined as "prefix %login suffix" in a single string, where "%login" is replaced by the user's login name.
- Find out which titles exist on the Intranet

### Titles Users
Link between users and titles.
- Find out which users have which titles and when they were added

### Transactions
Transactions are used to track the flow of evaluation points between users and pools, and the flow of Alterian Dollars between users and products in the Intra shop.
- Find out which users have donated evaluation points to the pool and when
- Find out which users have bought products in the Intra shop, for what price and when

### Translations
TODO

### User Candidatures
Privacy-sensitive information about a user, such as their phone number, e-mail address, home address, date of birth and emergency contact.
- Retrieve the home address of a user
- Retrieve the e-mail address of a user (though it is preferred to use their campus e-mail address instead (login@student.campus.tld))
- Retrieve the phone number of a user
- Retrieve the date of birth of a user
- Retrieve the emergency contact of a user and their contact information

### Users
Users are the core of the Intra. They are the students and staff that use the Intra.
- Find out which users exist on the Intra
- Get the login name, first and last name and full name of a user
- Get a link to a user's profile picture
- Check if a user is staff (`kind == "admin`)
- Get the amount of evaluation points a user has
- Check the date a user's data will need to be anonymized locally for GDPR compliance
- Check if a user has been alumnized or not
- Check when a user did the piscine (pool month and pool year)
- List a user's campuses, cursuses, languages, patronages, expertises and roles

### Waitlists
Waitlists for an event or exam that is full.
- Find out which users are on the waitlist for an event or exam and when they were added
- Find out how many users are on the waitlist for an event or exam

### Webhook Registeries
Webhook registeries are used to register webhooks for a campus. They are only available to staff.
> There is no way to retrieve registered webhooks with the API.
- Register a webhooks for a campus with a specific URL, defininig the events that should trigger the webhook
