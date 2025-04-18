# Control Yeelight para Android

Aplicación para controlar tiras LED Yeelight desde tu dispositivo Android.

## Requisitos

- Dispositivo Android con Node.js instalado (usando Termux)
- Tira LED Yeelight en la misma red WiFi
- Conocimiento de la IP de tu tira LED Yeelight

## Instalación en Android

1. Instala Termux desde la Play Store
2. Abre Termux y ejecuta los siguientes comandos:

```bash
pkg update
pkg install nodejs
pkg install git
```

3. Clona este repositorio:
```bash
git clone [URL_DEL_REPOSITORIO]
cd yeelight-control
```

4. Instala las dependencias:
```bash
npm install
```

5. Inicia el servidor:
```bash
npm start
```

## Configuración

1. Asegúrate de que tu tira LED Yeelight esté en la misma red WiFi que tu dispositivo Android
2. Modifica la IP en el archivo `server.js` (línea donde dice `192.168.1.26`) por la IP de tu tira LED
3. Abre el navegador en tu dispositivo Android y ve a `http://localhost:3000`

## Mantener el servidor activo

Para mantener el servidor activo en segundo plano:

1. En Termux, presiona el botón de menú y selecciona "Nueva sesión"
2. Ejecuta:
```bash
cd yeelight-control
npm start
```

3. Presiona el botón de menú y selecciona "Bloquear sesión"

## Solución de problemas

- Si la aplicación no se conecta, verifica que:
  - El servidor esté corriendo en Termux
  - La IP de la tira LED sea correcta
  - Ambos dispositivos estén en la misma red WiFi
  - La tira LED esté encendida

## Notas importantes

- Mantén Termux en segundo plano para que el servidor siga funcionando
- No cierres Termux completamente
- Si el servidor se detiene, reinicia Termux y vuelve a ejecutar `npm start` #   y e e l i g h t  
 