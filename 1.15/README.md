Commands I used to publish the existing docker-image devopsdockeruh/heroku-example to heroku. First I created a free account on heroku and install heroku cli on my machine./n

docker pull devopsdockeruh/heroku-example/n
heroku login/n
heroku container:login/n
docker tag devopsdockeruh/heroku-example registry.heroku.com/ddoan-heroku-example/web/n
docker push registry.heroku.com/ddoan-heroku-example/web/n
heroku container:release -a ddoan-heroku-example web/n

Click "Open App" on heroku, it will link to the heroku app was deployed: https://ddoan-heroku-example.herokuapp.com//n
