FROM java:8

ADD . /app

ENV M2_HOME /app

EXPOSE 8080

WORKDIR /app

RUN chmod a+x /app/mvnw

RUN /bin/bash -c '/app/mvnw -e install spring-boot:repackage -DskipTests'

CMD /app/mvnw -e spring-boot:run -DskipTests

