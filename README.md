# Distributed tracing with Spring cloud Jaeger
- Jaeger UI is not registering in spring-3.0. Working with 2.7.7

In this project I have figured out how we can integrate distributed tracing using spring cloud jaeger which is based on Opentracing.

## Jaeger Setup
- Start Jaeger using Docker

docker run -d --name jaeger-ui -p 16686:16686 -p 6831:6831/udp jaegertracing/all-in-one:latest

- Accessible at - http://localhost:16686/

## Endpoints
- /jaeger/client/{id} - Exposed in jaeger-client
- /jaeger/client/{id} - Exposed in jaeger-server. Connects to numbers api - numbersapi.com
