# Spring Cloud Config Server

## Introduction

Spring Cloud Config Server 실습 레포지토리입니다.

Config파일의 경우 아래 경로에 위치합니다.

[Spring Cloud Config File](https://github.com/spring-msa/Spring-Cloud-Config-File)

## Prerequisite

- Java 17
- kotlin 1.9.22
- Gradle 8.5


## Getting Started

### Local 환경에서 실행

아래 명령어를 통해 실행합니다.

```powershell
./gradlew bootRun
```

### Docker 환경에서 실행

아래 명령어를 통해 Docker 이미지를 빌드합니다.

```powershell
./gradlew bootBuildImage
```

아래 명령어를 통해 Docker 컨테이너를 실행합니다.

```powershell
docker run -d -e HOST_URL=http://host.docker.internal -it --name spring_cloud_config_server -p 8888:8888  spring-cloud-config-server:0.0.1-SNAPSHOT
```
