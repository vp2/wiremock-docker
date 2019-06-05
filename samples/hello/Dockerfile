FROM rodolpheche/wiremock

COPY wiremock-2.23.2-all.jar /var/wiremock/lib/wiremock-jre8-standalone.jar

COPY stubs /home/wiremock
#COPY wiremock-webhooks-extension-1.0.0-all.jar /var/wiremock/lib/

#COPY /Users/vp/wiremock-playground/wiremock-docker/wiremock-webhooks-extension-1.0.0-all.jar /var/wiremock/lib/


#ADD https://repo1.maven.org/maven2/com/opentable/wiremock-body-transformer/1.1.3/wiremock-body-transformer-1.1.3.jar /var/wiremock/extensions/

#ADD http://repo1.maven.org/maven2/org/wiremock/wiremock-webhooks-extension/1.0.0/wiremock-webhooks-extension-1.0.0.jar /var/wiremock/extensions/

CMD ["--extensions", "org.wiremock.webhooks.Webhooks"]

#CMD ["--extensions", "com.opentable.extension.BodyTransformer"]

CMD ["--local-response-templating"]