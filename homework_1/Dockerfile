ARG MAINTAINER="Andrii Shafran"
ARG VERSION="0.0.1"
ARG NAME="echo server by python"

# Create documentation
FROM debian
WORKDIR /app
RUN echo "Created image ${NAME}. Version ${VERSION}. Maintain by ${MAINTAINER}" 
RUN apt update && apt upgrade && apt install python3 -y && apt update

# Application image
FROM jmalloc/echo-server
COPY . .
EXPOSE 8080
