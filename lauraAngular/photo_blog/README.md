# Photo Blog

1. Clone the repository
2. Run `npm install`
3. Start the server `npm run serve`


#Notes for Project: 

// Note: Angular applications needs a module, and a module need a component
// Each of these needs metadata, and we use decorators to apply some configuration
// Modules & components are regular JS classes 
// Adding each component to the declarations is required! 

// You need 3 things for a component: a template (view), class and decorator (wires up class to template with metadata) 

// There are 3 main types of directives: Components, structural, and attribute.

// Components have a template

// Structural directives are a way to hide and reveal content inside of a component 

// Attrbibute directives are used the change the behavior/ apperance of an element (NgStyle)

// Also note the InMemory Web API service should only be used for Demo purposes, not for 'real' projects

#Angular LifeCycle Hooks:
    // Here are two examples: ngOnInit, ngOnDestroy 

 #//////////////////////////////////////////////////////////////////#   

  #Found In entry.service.ts file:

    // In the getEntries method, we're calling the HTTP service and pass in the  URL from the entries API, and reutrn a promise
    // Call the JSON method on the response, and then pick out the data object from the response
    // Define the type of data object by using TypeScript 'as' operator and assign the type of the Return value to an array of entries
    // Generics are insane, you have to make the getEntries return type valid
    // Generics begin with a type, in this case it's a Promise. 