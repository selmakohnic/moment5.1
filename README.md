# Moment 5.1 - Skapa REST-webbtjänst
I denna uppgift har en REST-webbtjänst med CRUD skapats, vars syfte är att lagra en lista med kurser. Denna lista presenteras i JSON-format. Webbtjänsten har skapats med objektorienterad PHP-programmering med en anslutning till en databasserver. 

För att starta systemet klona först projektet genom: **git clone https://github.com/selmakohnic/moment5.1.git**.

Följande curl requests kan användas för att testa REST-webbtjänsten:
* __GET:__ curl -i -X GET http://localhost/Webbutveckling3/Moment5/courselist.php/courses/
* __GET med ID:__ curl -i -X GET http://localhost/Webbutveckling3/Moment5/courselist.php/courses/1
* __POST:__ curl -i -X POST -d '{"code":"DT057G","name":"Webbutveckling I", "progression":"A", "syllabus":"https://www.miun.se/utbildning/kursplaner-och-utbildningsplaner/Sok-kursplan/kursplan/?kursplanid=17948"}' http://localhost/Webbutveckling3/Moment5/courselist.php/courses/
* __PUT:__ curl -i -X PUT -d '{"code":"DT057G","name":"Webbutveckling I", "progression":"A", "syllabus":"https://www.miun.se/utbildning/kursplaner-och-utbildningsplaner/Sok-kursplan/kursplan/?kursplanid=17948"}' http://localhost/Webbutveckling3/Moment5/courselist.php/courses/1
* __DELETE:__ curl -i -X DELETE http://localhost/Webbutveckling3/Moment5/courselist.php/courses/1

Demonstration av uppgiften hittas här: http://studenter.miun.se/~seko1800/dt173g/moment5.1/courselist.php/courses