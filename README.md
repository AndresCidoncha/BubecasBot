# BubecasBot
Bot de telegram para recibir notificaciones en tiempo real del cambio de estado de tu beca y para consultar su estado. 
El sistema te preguntará si deseas que se almacene una relación entre tu ID de Telegram y tu DNI para avisarte en caso de cambio del estado de tu solicitud de beca.
En caso de no querer que se almacenen estos datos puede rechazarse, pero no se recibirán avisos en tiempo real del cambio de estado. 
Aún así, podrá usarse para consultar el estado de la beca pasando a los comandos el DNI como parámetro.

Usa [Bubecas](http://193.145.111.205/bubecas.htm) para obtener la información.
Usa [Python Bot API](https://github.com/python-telegram-bot/python-telegram-bot).

##Uso
/start - Inicia el bot con el asistente de notificacion en tiempo real.
/setDNI <DNI> - Especifica tu DNI al sistema para activar las notificaciones en tiempo real.
/status [DNI] - Obtiene solo el estado (Denegada, propuesta para pago: X euros, etc) de la solicitud. Si se pasa un DNI como parámetro consultará las solicitudes del DNI indicado.
/info [DNI] - Obtiene toda la información acerca de la solicitud. En caso de pasar un DNI como parámetro, devolverá la información de la solicitud del DNI indicado.
/stop - Detiene el servicio del bot y elimina los datos almacenados de tu usuario (relación ID-DNI).
