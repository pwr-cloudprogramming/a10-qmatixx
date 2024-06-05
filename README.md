# Mateusz Luberda

- Course: Cloud programming
- Group: PN 9:15
- Date: 27.05.2024

## Environment architecture

VPC, podsieci, tablice routingu, security gropus, instancja ec2 oraz Cogntio.

## Preview

Screenshots of configured AWS services. Screenshots of your application running.

EC2
![EC2](img/ec2.png)
Kółko i krzyżyk
![App running](img/game1.png)
![App running](img/game2.png)
Cognito
![Cognito](img/cognito.png)
Congig.js
![Config.js](img/config.png)

## Reflections

Do wykonania zadania wykorzystałem plik main.tf z zadania A5. Najpierw stworzyłem autentyfikację Cognito, wyklikując kolejne opcje w AWS-ie. Próbując przenieść to na kod terraforma, największe trudności napotkałem z odświeżaniem tokenów oraz zapisywaniem użytkowników. Poza tym skrypt users_data jest prawie taki sam, jak przy zadaniu A5.
