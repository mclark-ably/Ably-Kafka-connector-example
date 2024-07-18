Example usage

1. Rename docker-compose-connector.properties.example to docker-compose-connector.properties
2. Add Ably API key to client.key
3. run docker compose up -d
4. Run Kafka_connector % docker compose exec -T kafka kafka-console-producer --topic kafka-connect-ably-example --broker-list kafka:9092 << EOF
   message 1
   message 2
   message 3
   EOF
