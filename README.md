# iobuilders
## POC EXERCISE
### (1) What are your thoughts, ideas about tech, architecture with this context?

Being a Finance App in which the users are going to manage money and have their identity in, the security is one of the main issues we should have in mind. On the other hand we also want this project to be a base project for other ins the company so it has to be well design in a way that reaching it’s services from other projects or extending the services should be simple and barely affect the development that has been done before.
For tackling these issues, I think, after the research I have been doing these days, that the best architecture for the core of this project is Hexagonal Architecture or Domain Driven Development (DDD).
The reason for me to think this way is because:
1. We want it to be the base for future projects and this type of architecture abstracts through adapters everything that it outside of our model.
So if for example, after creating the mobile app we decide that we want to do the same but with a web app and that the data that is send comes with another format we just need to create a new adapter that adapts the data into the object that our model works with.
This allows us to change the persistence technology or the type of ERC token we want to use without affecting our business logic.

1. This type of architecture also allows you to have more control of the code because once you have your business logic you barely have to touch it making it easier to control bugs or security flaws that can come with those bugs.

It has drawbacks too, it is a bit slow at the beggining and it needs a good design for it but I think that if you want to have something as a base for future projects of the company you have to try and do it correctly from the beginning.

The technologies should be chosen depending on the team we have available but I think that for the Front end part of the project we could go with Angular and Ionic as a framework because Angular components are highly reusable and ionic allow us to have the app running in ios and android at the same time without needing to develop both app separately. For the backend Java/Kotlin/Groovy with Spring boot will work, specially having in mind that the company works with Groovy, but also, we could have in mind using python with Django because of how fast and versatile it is.

### (2) Describe the skills, roles and team size, that you think is the best fit for this project.

Regarding the team, we must consider that the POC has 4 months to develop the project and the code must be as clean as possible because we want it to be usable for other projects.

Front-end: 1 senior developer with experience in organising the front-end code with 1 or 2 less experience developers that can be autonomous. This part of the team should focus in creating the apps with a simple style layout, so they have more time for testing coverage and having the project organise and clean for reuse.
Back-end: 1 senior developer with experience in architecture to be the “go to” to clear doubts about it with 3-5 less experience developer in which we can include one or 2 more junior ones that can do some tasks more independently.

UX/UI: If we take the approach of not focusing time in the style we don’t need any one during the POC, after we see that the project works we could add this member to the team of have one in the team that continue the project. This is because styling apps or webs is one of the most time-consuming parts of a project and time is something that this POC don’t have.
