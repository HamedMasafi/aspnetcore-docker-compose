# ASP.NET Core & Sql server docker compose 

## Usage
Change variables values in env.sh file (if needed)

| Variable name   | Descript                          | Default value |
|-----------------|-----------------------------------|---------------|
| PORT            | Port of webserver                 |            80 |
| APP_DIR=./app   | Directory for website             |         ./app |
| SA_PASSWORD     | Password for sql server sa        |     sap123456 |
| DATA_DIR=./data | Directory path for database files |        ./data |


### Create new docker-compose file
Run this script:
```
./init
```

After this file docker-compose.yml will be created (or updated)

### Create new project
```
./new_site mvc --auth Individual
```

Edit your site placed into ./app directory

### Run project

```
docker-compose build
docker-compose up -d 
```

Visit http://127.0.0.1:5000 

Note: the port 5000 can be changed in env.sh file
