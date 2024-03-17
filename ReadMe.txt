To Run App
==========

(1) Start Kafka Server/Broker in a console (Location: Kafka sourse location)
    ========================================
	(i) Download and unzip Kafka sourse
	(ii) Run below commands in that source loaction 

		.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties

		.\bin\windows\kafka-server-start.bat .\config\server.properties


(2) Start Both Application
(3) Send request for Producer App




---------------------------------------------------------------------------------------------------------------------------------------------------------------
Without running both Produser and Consumenr app, you can try prduser and consumer in below way


In ProduserConsole
==================
C:\kafka\bin\windows>kafka-console-producer.bat --broker-list localhost:9092 --topic test

{"Name":"Kamal", "Age":24, "Gender": "male"}


In ConsumerConsole
==================
C:\kafka\bin\windows>kafka-console-consumer.bat --topic test --bootstrap-server localhost:9092 --from-beginning




