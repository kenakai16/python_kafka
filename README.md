# python_kafka

## FROM neo4j:4.0.1-enterprise

## MAINTAINER Utop_AI_2020

## ENV APOC_URI=https://github.com/neo4j-contrib/neo4j-apoc-procedures/releases/download/4.0.0.7/apoc-4.0.0.7-all.jar
## ENV POSTGRES_URI=https://github.com/microsoft/mssql-jdbc/releases/download/v8.2.2/mssql-jdbc-8.2.2.jre8.jar

## ADD --chown=neo4j:neo4j ${APOC_URI} plugins
## ADD --chown=neo4j:neo4j ${POSTGRES_URI} plugins

## ENV NEO4J_ACCEPT_LICENSE_AGREEMENT=yes
## ENV NEO4J_dbms_security_procedures_unrestricted=apoc.*
## ENV dbms.memory.heap.initial_size=3G
## ENV dbms.memory.heap.max_size=3G
## ENV dbms.memory.heap.max_size=3G
## ENV dbms.logs.debug.level=DEBUG

## EXPOSE 7473/tcp 7474/tcp 7687/tcp

## ENV NEO4J_AUTH=neo4j/test

## CMD ["neo4j"]
