Commands I used to publish the existing docker-image devopsdockeruh/heroku-example to heroku. First I created a free account on heroku and install heroku cli on my machine. <br/>

docker pull devopsdockeruh/heroku-example <br/>
heroku login <br/>
heroku container:login <br/>
docker tag devopsdockeruh/heroku-example registry.heroku.com/ddoan-heroku-example/web <br/>
docker push registry.heroku.com/ddoan-heroku-example/web <br/>
heroku container:release -a ddoan-heroku-example web <br/>

Click "Open App" on heroku, it will link to the heroku app was deployed: https://ddoan-heroku-example.herokuapp.com/ <br/>
