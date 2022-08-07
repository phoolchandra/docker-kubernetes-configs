FROM confluentinc/cp-kafka-connect:7.1.0-1-ubi8

RUN confluent-hub install  --no-prompt debezium/debezium-connector-mysql:1.9.3 \
   && confluent-hub install --no-prompt debezium/debezium-connector-postgresql:1.9.3 \
   && confluent-hub install --no-prompt debezium/debezium-connector-mongodb:1.9.3 \
   && confluent-hub install --no-prompt confluentinc/kafka-connect-s3:10.0.11 \
   && confluent-hub install --no-prompt confluentinc/kafka-connect-s3-source:2.2.3 
