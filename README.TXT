This repository contains libraries that are required by the bundle org.openhab.io.multimedia.tts.marytts
They were outsourced here in order to keep the size of the main repo small as these libraries are quite huge.

This Repo is meant to be (locally web) hosted so the openHAB compile using discontinued repo's as referred in pom.xml can continue.
This is specifically valid for and to recompile discontinued openHAB version 1 addons
- openhab1-addons-1.13.0
- openhab1-addons-1.14.0-SNAPHOT
- a.s.o.

using: $  mvn clean install -DskipTests=true -DskipChecks -o -e -X -pl :org.openhab.io.multimedia.tts.marytts
Note: inside pom.xml we changed forced dependency library references 
	from:	https://bintray.com/artifact/download/openhab/3rd/ 
	to : 	https://github.com/ptrooms/openhab.dependencies/raw/qnap/

Alternatively we could have used the original at https://github.com/yilmazogras/openhab.dependencies/raw/master/

