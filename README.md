# Position-Simulator

## TEST APPLICATION 

1. Build Docker Image of position-simulator  
2. docker run -d -p 8161:8161 -p 61616:61616 --name myqueue --network locationtracker mooneshkachroo/activemq:0.0.1-RELEASE
3. docker run --network locationtracker --env spring.activemq.broker-url=tcp://myqueue:61616 --env fleetman.position.queue=positionQueue mooneshkachroo/position-simulator:0.0.1-RELEASE


## BUILD CONTAINER FOR ActiveMQ QUEUE
1. In cmd prmpt > navigate to activemq folder 
2. Build image > >docker image build -t mooneshkachroo/activemq:0.0.1-RELEASE .




## SETTING UP GIT REPO
1. Move to lt-position-simulator folde in cmd prompt
2. git init
3. Go to Github and create repository lt-position-simulator
4. git remote add origin https://github.com/moonesh/lt-position-simulator.git
5. git add .
6. git commit -m""
7. git push --set-upstream origin master  

