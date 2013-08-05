heroku-jetty-spring-mvc
=======================

Heroku-friendly Java web app skeleton using Spring MVC. 

Probably the easiest way to get a public Java webapp up and running.

##How to use

1. Create a [Heroku](http://www.heroku.com/) and install the [Heroku Toolbelt](https://toolbelt.heroku.com/)
1. Clone this repo.
1. Create a Heroku app:
```
heroku create
```
1. Deploy:
```
git push heroku master
```
1. Access your app:
```
heroku open
```

##Running locally

There are two options here:

### Using maven

```
mvn jetty:run
```

That will start a server running on [http://localhost:5000](). You can change the configuration by editing the *jetty-maven-plugin* inside the *pom.xml*.

### Using foreman

```
foreman start
```

This will start a server running on [http://localhost:5000](). You can change the configuration by editing the *Procfile* file.

##Accessing logs

The app is configured to use logback. Once the app is running on Heroku, you can access logs via:

```
heroku logs
```

##Troubleshooting

The app uses a very simple and standard configuration for Spring. But if you have any trouble with it feel free to open an issue here or just ping me on [twitter](http://www.twitter.com/s4nchez).
