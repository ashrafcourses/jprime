[![Build Status](https://travis-ci.org/ashrafcourses/jprime.svg?branch=master)](https://travis-ci.org/ashrafcourses/jprime)

mvn archetype:generate -DarchetypeArtifactId=jersey-heroku-webapp \
                -DarchetypeGroupId=org.glassfish.jersey.archetypes -DinteractiveMode=false \
                -DgroupId=dal.cources -DartifactId=jprime-webapp -Dpackage=dal.jprime \
                -DarchetypeVersion=2.25

 travis encrypt $(heroku auth:token) --add deploy.api_key
