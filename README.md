# sit323-737-2023-t1-prac5p

## Starting application

TO install node modules run the following command
`npm install`

Run the following command to build and run the project using docker-compose
`docker-compose up -d`

To test connection use the to the following URL
`http://localhost:8080/getToken`

## To test the health check

sh into the container using the following command
`docker exec -it sit323-737-2023-t1-prac5p-web-1 sh`

Find the process ID of the node application using the following command
`ss -lptn 'sport = :5000'`

kill the procss using the following command
`kill <pid>`

The process will be killed but restarted immediately.
Check logs in docker container to view the process.
