Para correr la app:

1) Instalar NodeJS

   http://nodejs.org/

2) Instalar Ionic/Cordova

   npm install -g cordova ionic


Para que los mensajes PUSH puedan funcionar:

1) Instalar Ionic Cloud y seguir todas las instrucciones de este enlace:

	http://docs.ionic.io/setup.html

2) Una vez instalado, importar el proyecto en Google Firebase. Luego copiar el key y usarlo en los servicios PUSH:

	https://console.firebase.google.com/

3) Probar los servicios usando una herramienta como Postman, usando la documentación de Ionic:

	http://docs.ionic.io/api/endpoints/push.html


Para instalar los plugins del lector QR:

1) Instalar el plugin de ngCordova:

	http://ngcordova.com/docs/install/

2) Luego instalar el plugin del lector de QR:

	http://ngcordova.com/docs/plugins/barcodeScanner/

Es importante saber que si ejecutas el proyecto desde el browser, siempre te va a decir "error: cordova not defined" porque el objeto "cordova" sólo se crea desde un dispositivo real.


PARA DESCARGAR ARCHIVOS PDF:

1) Ya teniendo ngCordova instalado, se debe instalar el siguiente plugin para permitir la descarga de archivos:

	cordova plugin add cordova-plugin-file-transfer

2) Y este otro plugin para poder abrirlos con la app por defecto del dispositivo:

	cordova plugin add https://github.com/pwlin/cordova-plugin-file-opener2.git


PARA CARGAR LAS FOTOS EN MI PERFIL:

1) Se debe instalar el plugin de la camara para tomar fotos o seleccionar una de la biblioteca de imagenes del dispositivo:

	cordova plugin add cordova-plugin-camera


PARA ABRIR ENLACES EXTERNOS:

cordova plugin add cordova-plugin-inappbrowser

PARA ESTILIZAR LAS NOTIFICACIONES PUSH:

npm install sweetalert


ANGULAR MATERIAL: (para el spinner circle en la Trivia)

	1) npm install angular-material --save
	2) npm install angular-animate --save
	3) npm install angular-aria --save


SPLASH SCREEN

	1) El splash debe medir 2208x2208 porque si es mas grande, no va a funcionar. Una vez generado el splash y guardado en la carpeta /resources, se debe ejecutar:

ionic resources --splash


ICONOS


