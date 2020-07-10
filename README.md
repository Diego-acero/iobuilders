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
