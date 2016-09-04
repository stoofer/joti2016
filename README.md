# joti2016
Playing with docker and nodes to see if we can have something interesting for JOTI 2016

TODO
- install mongo-db
- install node-RED
- configure data volumes
- design twitter flow to db
- design web page flow


to start nodered-joti:
docker run -it -p 1880:1880 --name jnr nodered-joti


Record contacts
serve web form -> post contact to node red via WS -> store in mongo

Identify location
form should provide geolocation lookup

Tweet contact details
- post new contact to twitter

Draw map
serve status page -> connect via WS -> read all contacts so far
                                    -> listen for new contacts

Bisley watcher
- listen to twitter for #baughurstShooters
-> record to mongo
-> stream to tweet monitor page

Deploy to PI
- get docker image working on rpi
Hook up the IO pins to a bread board and get it to light something up
