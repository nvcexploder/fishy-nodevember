# Nodevember Microsoft Cephalopod Code Challenge

## Wait, what?

This is an easy way to enter into the Microsoft Azure Nodevember Competition! 

There is an easier way, from [Sarah Sexton](https://github.com/SarahSexton) here: [Microsoft Azure](https://github.com/SarahSexton/NodevemberMS/blob/master/README.md)

The difference here is that you'll need to set up your Azure account, add an app, and add a new Azure remote to which you can push your code. A good tutorial can be found [here](http://blogs.msdn.com/b/sarahsays/archive/2015/08/31/building-your-first-node-js-app-and-publishing-to-azure.aspx) and [here](https://azure.microsoft.com/en-us/documentation/articles/web-sites-nodejs-develop-deploy-mac/)

## Whatsit do?

If you hit the root URL, you'll be given the taxonomic data for the Class Cephalopoda Cuvier. 

## How's it work? 

It uses [hapi.js](http://hapijs.com) to create a server that returns a JSON representation of the Cephalopods. 

## IMPORTANT NOTE

When creating a server, you need to assign it a port. Azure will assign your port to you, and the way to access that can be found here:

```javascript
const port = process.env.PORT || 8080;
```

What's happening here is that Azure is setting the port number in the environment variable 'PORT', and the application is reading that. If it's not set, the port defaults to '8080'.

Good luck!