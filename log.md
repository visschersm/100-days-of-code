# 100 Days Of Code - Log

### Research Ideas
- Dapr
- Dapper
- MongoDb
- AWS
- Design patterns
- Golang
- F#
- C++ OpenGL/DirectX 11- Graphics Framework
- TDD form strong opinion on how it should be done
- C# Attributes
- Proper (custom)Exception creation and handling 

### Day 0: Januari 22 2021

Preparing for the 100-days-of-code challenge.
Before starting this challenge i'm gathering some possible research ideas.

**Today's Progress**: Started with a small C# DotNet 5.0 project in which I'm going to setup up a Dapper ORM connection. I created an Azure SQL Server to test with a real setup. But I'm struggling a bit because my SQL knowledge is really basic. Spend a bit more time than the hour on getting it to work, but the first data was written to the database.

**Link(s) to work:** [Dapper Tryout](https://github.com/visschersm/dapper-tryout)

### Day 1: Januari 23, 2020

**Today's Progress**: Created a dotnet webapi project with some libraries to tryout different ORMs. In the next few days I will work on an implementation on DAPPER ORM and comapre it with some EFCore implementation. Since EF is my mainly used ORM I will compare it with EF. I also want to create an implementation of LLBLGen since I heard of that last year and want to get familiar with that one as well.

**Link(s) to work**: [ORM Tryout](https://github.com/visschersm/orm_api_test)

### DAY 2: Januari 24, 2021

**Today's Progress**: Created an TodoController which is going to contain some basic CRUD to test the different ORMs against. Started with Dapper to see if I can already manage basic CRUD with this ORM. I might want to get into seeing how I can manage different build configs to support demoing better. Something like: Run with Dapper/Run with EF to start the project running on a different ORM. "CROSS_ORM"?
I think it is much fun to finally learn some more SQL. Only had to use it in very minimal ways because with EntityFramework I have almost never had to use it. 

**Link(s) to work**: 
1. [ORM Tryout](https://github.com/visschersm/orm_api_test)
2. [Postman CRUD](https://www.getpostman.com/collections/77266b4c01a76c51ef8a)

### DAY 3: Januari 25, 2021

**Today's Progress**: Today I worked on the CRUD implementation of EFCore and LinqToDb. I created an EFCore, since this is my most used ORM, to verify results, and compare how other ORMs are used to something i'm used to myself. Maybe tomorrow I can start setting up some build configs or start on a LLBLGen implementation. After that I'll probabbly start working on more advance implementations/usecases. 

**Link(s) to work**: 
1. [ORM Tryout](https://github.com/visschersm/orm_api_test)
2. [Postman CRUD](https://www.getpostman.com/collections/77266b4c01a76c51ef8a)

### DAY 4: Januari 26, 2021

**Today's Progress**: Today I worked on an implementation of NHibernate. So far this was the most problamatic for me to setup. The docs felt a bit old and the way it was setup did not seem to match dotnet core exactly. In the end found a nice blog which filled in the missing pieces. Still needs some work to fine tune the implementation but the basic CRUD operations are done.

**Link(s) to work**: 
1. [ORM Tryout](https://github.com/visschersm/orm_api_test)
2. [Postman CRUD](https://www.getpostman.com/collections/77266b4c01a76c51ef8a)
3. [Blog mentioned](https://gunnarpeipman.com/aspnet-core-nhibernate/)

### DAY 5: Januari 27, 2021

**Today's Progress**: Today I worked on an implemenation of LLBLGen orm. It took me a while before I had everything setup but managed to implement the CRUD operations in the end. Want to invensigate if there are more direct ways to configure the llblgen model to generate the entities. Now I would have to change the projects. Would be nice if the model can be synced automatically with the solution in which I am using it. Read something about that it should be managable from within visual studio.
Next to that started on a TPT inheritance implementation within the EFSample. Going to expand this to the other services.

**Link(s) to work**:
1. [ORM Tryout](https://github.com/visschersm/orm_api_test)
2. [Postman CRUD](https://www.getpostman.com/collections/77266b4c01a76c51ef8a)

### DAY 6: Januari 28, 2021

**Today's Progress**: Today I started implementing TPT inheritance. EFCore 5 now supports it out of the box so that was pretty easy. Trying to get it to work in Dapper however is a different story. I think I managed to get the Create method working had to do some googling though. 

**Link(s) to work**:
1. [ORM Tryout](https://github.com/visschersm/orm_api_test)
2. [Postman CRUD](https://www.getpostman.com/collections/77266b4c01a76c51ef8a)


### DAY 7: Januari 29, 2021

**Today's Progress**: Today I created some different build configurations. Now it is more easy to run different ORM setups like shown in the following image:

![alt text](https://github.com/visschersm/100-days-of-code/blob/master/supported-orms.png?raw=true)

Using launch settings it was rather easy to create these configuations which make it possible to configure all the different ORM implementations and run them with a button click. Next to that I worked on different TPT inheritance implementations. I want to see what is possible with the different ORMs and how they compare to eachother esppecially in usablility. After the inheritance implementation I want to tryout many to many relationships. 

1. [ORM Tryout](https://github.com/visschersm/orm_api_test)
2. [Postman CRUD](https://www.getpostman.com/collections/77266b4c01a76c51ef8a)

### DAY 8: Januari 30, 2021

**Today's Progress**:Today I worked some more on the implementation details of the AnimalService to test TPT inheritance in different ORMs. I also added task.json for VSCode so I can run the application more easily configured with the different ORMs.
|ORM|TPT Working/Checked|
|---|---|
|Dapper|<ul><li>- [x] </li></ul>|
|EFCore|<ul><li>- [X] </li></ul>|
|Linq2Db|<ul><li>- [ ] </li></ul>|
|LLBLGen|<ul><li>- [ ] </li></ul>|
|NHibernate|<ul><li>- [ ] </li></ul>|
