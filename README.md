# java-web-api-maven-spring-zuul-zipkin-prometheus

## Description
A springboot app that uses zuul
as a reverse proxy. All requests
to `/api` will be forwarded to nodejs
server. Uses prometheus to import data
from zipkin logs.

## Tech stack
- java
- maven
  - springboot
  - netflix zuul
- nodejs
- prometheus

## Docker stack
- openjdk:11-jdk
- node:latest
- prom/prometheus

## To run
`sudo ./install.sh -u`
- ZIPKIN DASHBOARD http://localhost
- API http://localhost:81/all
- REMOTE API http://localhost:81/api/all
- PROMETHEUS DASHBOARD http://localhost:82

## To stop
`sudo ./install.sh -d`

## For help
`sudo ./install.sh -h`

## Credits
- https://spring.io/guides/gs/routing-and-filtering/
