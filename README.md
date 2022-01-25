# heroku_test

Follow the instructions below to deploy to Heroku

1. Create your SpringBoot application. Run and test it locally.
2. Add 'server.port=${PORT:8080}' to your application.properties file
3. Create your Dockerfile. Use Dockerfile from the root of this project as a example
4. Create docker image with 'docker build -t springbootapp .' command
5. Run it locally with 'docker run -p 8080:8080 -t springbootapp'
6. Create Heroku account: https://www.heroku.com/
7. Install the Heroku CLI and log in using the CLI 'heroku login'
8. Run 'heroku container:login'
9. Run 'heroku create [APP]' ([APP] - name of your own app)
10. Run 'heroku container:push web --app=[APP]'
11. Run 'heroku container:release web --app=[APP]'
12. Run 'heroku open --app=[APP]' and test your app :)



# P.S.

Add a maven plugin to your pom.xml if you don't want to deal with MANIFEST.MF.
See pom.xml at the root of this project
