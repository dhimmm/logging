# MySQL Slow Query Log with ELK and Graylog

This project demonstrates how to configure MySQL slow query logs with ELK (Elasticsearch, Logstash, Kibana) and Graylog using Docker Compose.

## Setup

1. Clone the repository.
2. Update the `.env` file with the correct environment variables.
3. Run `docker-compose up --build` to start all services.
4. Access Kibana at `http://localhost:5601` and Graylog at `http://localhost:9000`.

## Testing Performance

You can change the `long_query_time` setting in `mysql/my.cnf` to `0`, `1`, or `10` to see how it affects performance.

## Accessing Logs

- Kibana: Go to the Kibana dashboard and view logs in Elasticsearch.
- Graylog: Use the Graylog interface to search and filter MySQL slow query logs.
