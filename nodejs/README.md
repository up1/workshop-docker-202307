# Run with nodejs
```
$npm install
$npm start
```
URL = http://localhost:3000

## Working with docker
```
$docker image build -t my_node .
$docker image build -t my_node -f Dockerfile .
$docker container run -d -p 3000:3000 my_node
```