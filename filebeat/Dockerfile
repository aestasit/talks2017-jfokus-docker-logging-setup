FROM busybox

COPY filebeat-5.2.0-linux-x86_64/filebeat /filebeat
COPY filebeat-5.2.0-linux-x86_64/filebeat.template.json /filebeat.template.json
COPY filebeat-5.2.0-linux-x86_64/filebeat.template-es2x.json /filebeat.template-es2x.json
COPY filebeat.yml /filebeat.yml

CMD ["/filebeat", "-e", "-d", "*", "/filebeat.yml"]

