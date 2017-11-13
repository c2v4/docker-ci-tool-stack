FROM sonarqube:6.6

RUN 	apt-get update \
	&& apt-get install -y git

RUN 	git clone https://github.com/arturbosch/sonar-kotlin /tmp/sonar-kotlin/ && \
	cd /tmp/sonar-kotlin && \
	./gradlew build && \
	cp build/libs/$(ls build/libs) /opt/sonarqube/extensions/plugins


