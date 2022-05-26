# MongoDbWrapper



## Getting started

Wrapper designed to be used to interact with a MongoDB database.

## Integrate with your tools

Declare dependeny injection in Startup.cs :

-ServiceActivator.Configure(app.ApplicationServices) in Configure(IApplicationBuilder app, IWebHostEnvironment env)

-Add ServicesCollectionExtension.AddMongodbWrapperConfiguration() to ServicesCollection

-Declare as many BaseRepository as Documents : services.AddTransient<IBaseRepository<AuthorDocument>, BaseRepository<AuthorDocument>>(); 
