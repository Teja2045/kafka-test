# kafka-test

A simple kafka test application with a broker built from docker image

#### run broker
    docker-compose up -d

#### run producer
     go run cmd/producer/producer.go

    
#### run consumer
    go run cmd/consumer/consumer.go


#### Send Message / event
    curl -X POST http://localhost:8080/send \
    -d "fromID=1&toID=4&message=Lena liked your post: My weekend getaway!"

#### Get Notifications
    curl http://localhost:8081/notifications/4


Source: https://www.freecodecamp.org/news/build-a-real-time-notification-system-with-go-and-kafka/
