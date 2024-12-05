# Today I learned... 04/12/24

This is a MD training

## I learned the use of 'ctx' in a AdonisJS project

While following a lesson on AdonisJS6, when making the routes we had to use the 'ctx' object.

### But what is 'ctx' then ?

Well, it was use in that context :

```ts
route.get('/movies', async (ctx) => {
return 'My awesome Movie!'
})
```

'ctx' stands for context, it's an object provided by the framework AdonisJS, it contains information about the incoming HTTP request and outgoing HTTP response. So, everything I need to handle the request and craft a response !

### Why is ctx important ?

It makes working with requests and responses easier by putting all the important information in one place. Depending on the framework, the structure of ctx may vary, but it still will have the same job : **to represent the context of the current HTTP request and response cycle.**

So yes, this is what I learned today ! :)
