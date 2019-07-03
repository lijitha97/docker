FROM maven:3.5-jdk-8-alpine as build

RUN mkdir /refertalents

RUN mkdir /refertalents/files

WORKDIR /refertalents

COPY . .

RUN mvn install

WORKDIR target/

CMD ["java","-jar","/refertalents/target/ReferTalents-0.0.1-SNAPSHOT.jar"]
