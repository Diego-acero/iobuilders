# iobuilders
## POC EXERCISE
### (1) What are your thoughts, ideas about tech, architecture with this context?

Being a Finance App in which the users are going to manage money and have their identity, the security is one of the main issues we should have in mind. On the other hand we also want this project to be a base project for other projects in the company so it has to be well design in a way that reaching its services from other projects or extending the services should be simple and barely affect the development that has been done before.
For tackling these issues, I think, after the research I have been doing these days, that the best architecture for the core of this project is Hexagonal Architecture or Domain Driven Development (DDD).

The reason for me to think this way is because:

1.	We want it to be the base for future projects and this type of architecture abstracts through adapters everything that it outside of our model.
So if for example, after creating the mobile app we decide that we want to do the same but with a web app and that the data that is send comes with another format we just need to create a new adapter that adapts the data into the object that our model works with.
This allows us to change the persistence technology or the type of ERC token we want to use without affecting our business logic.

2.	This type of architecture also allows you to have more control of the code because once you have your business logic you barely have to touch it making easier to control bugs or security flaws that can come with those bugs.
It has drawbacks too, it’s a bit slow to start this development and it needs a good design for it but I think that if you want to have something as a base for future projects you have to try and do it correctly from the beginning.

The technologies should be chosen depending on the team we have available but I think that for the Front end part of the project we could go with Angular and Ionic as a framework because Angular components are highly reusable and ionic allow us to have the app running in ios and android at the same time without needing to develop both app separately. For the backend Java/Kotlin/Groovy with Spring boot will work, specially having in mind that the company works with Groovy, but also, we could consider using python with Django because of how fast and versatile it is.


### (2) Describe the skills, roles and team size, that you think is the best fit for this project.

Regarding the team, we must consider that the POC has 4 months to develop the project and the code must be as clean as possible because we want it to be usable for other projects.

Front-end: 1 senior developer with experience in organising the front-end code with 1 or 2 less experience developers that can be autonomous. This part of the team should focus in creating the apps with a simple style layout, so they have more time for testing coverage and having the project organise and clean for reuse.

Back-end: 1 senior developer with experience in architecture to be the “go to” to clear doubts about it with 3-5 less experience developer in which we can include one or 2 more juniors that can do some tasks more independently.

Manager/Product Owner: We need 1 manager/product owner to organise and prioritise the tasks.

UX/UI: If we take the approach of not focusing time in the style we don’t need any one during the POC, after we see that the project works we could add this member to the team or have one in the team that continues the project. This is because styling apps or webs is one of the most time-consuming parts of a project and time is something that this POC do not have.

### (3) Go into the details, about which tech/business methodologies, tools, etc..., you think fit best to the scenario, and the culture you like and makes sense to apply on this company

Nowadays nearly all the Software development teams have work with Agile methodologies so I think it would be a good idea to use Kanban or Scrum (if the team has no experience with Kanban because it can take some time to get use to this methodology). For the board I will use Jira, easy to organise and to use by the team.

About the team: 

- We need the team to help each other, creating an atmosphere of trust so everyone feels comfortable asking questions if they doubt about something.

- No blaming culture, if something goes wrong, we do not look for someone to blame but instead for a solution for that situation.

- Everyone can give their opinion backing it up with reasons, sometimes we think that just the ones with more experience can give a good opinion about problem solving but less experience developers can give out of the box ideas that can be really helpful and can inspire others to get those ideas and improve them with the experience they have.

- Ownership, each member of the team must feel part of it, so they take also the ownership of each task, test… they do during the POC.

- Code Review mentality, after finishing each task someone has to CR the commits to check if there are bugs or if the code can be improved. This helps everyone to be humbler, helps learning and makes code cleaner.

- Master only, if the team is organised and know how to use git correctly master only approach is the best way to fast commit and have no big merging conflicts that can take some time to solve. For this we need to have the team with a micro commit mentality making them know that is better to create smaller commits than big commits that are difficult to follow in CR or coding conflict situations.

- 1to1 meetings with manager/product owner/figure in charge of the POC, during my internship I felt that this meetings were really helpful for everyone because they were a safe place were you could talk about how you were feeling in the team, with the project, with your teammates… making it easier to cope with the team problems before they start to emerge.
