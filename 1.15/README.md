Commands I used to publish the existing docker-image devopsdockeruh/heroku-example to heroku. First I created a free account on heroku and install heroku cli on my machine.

docker pull devopsdockeruh/heroku-example
heroku login
heroku container:login
docker tag devopsdockeruh/heroku-example registry.heroku.com/ddoan-heroku-example/web
docker push registry.heroku.com/ddoan-heroku-example/web
heroku container:release -a ddoan-heroku-example web

Click "Open App" on heroku, it will link to the heroku app was deployed: https://ddoan-heroku-example.herokuapp.com/