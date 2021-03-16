# Angular-Universal-SSR-Example

This project was created due to the lack of angular-universal SSR demo projects

Inspired by: https://stackoverflow.com/q/66639936/3712531

____

# 1 installation

select your folder and open cmd or git bash and execute the command 
`git clone https://github.com/StanlyLife/Angular-Universal-SSR-Example.git`

# 2 Starting the project

**DotNet**

Open the sln and run the project.
Do *not* start the project on IIS without configuring the environment variables (`url` variable) in `Angular-SSR/src/environments/environment.ts`

**Angular**

If you want to run the project without SSR use the command:
`ng serve`

if you want to run the project with SSR use the command:
`ng run ModernaMediaAngular:serve-ssr`

____

# 3 verifying that SSR works

there are sevral differnt ways to check if the page is pre-rendered
1. check the websites html elements: https://flaviocopes.com/nextjs-ssr/
2. My favorite way is by disabling javascript in devtools: https://stackoverflow.com/a/35323885/3712531

____
____
____

# How it works

Freecodecamp has a great blog post on server side rendering (vs client side rendering)

https://www.freecodecamp.org/news/what-exactly-is-client-side-rendering-and-hows-it-different-from-server-side-rendering-bd5c786b340d/#:~:text=Server%2Dside%20rendering%20is%20the,the%20contents%20of%20the%20website.

Below you can see an example of client side rendering.
As you can see there is a small delay between html load and the api/http request content load

![image](https://user-images.githubusercontent.com/13099896/111300247-25d32680-8651-11eb-88c6-6b12e97a00a2.png)


For more info check out: https://angular.io/guide/universal
