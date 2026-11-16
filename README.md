<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=200&section=header&text=Bot-Lavalink-Simple&fontSize=70&fontAlignY=35&animation=twinkling&fontColor=gradient" alt="Bot-Lavalink-Simple Header"/>

  <p>
    <img src="https://img.shields.io/badge/Estado-Archivado-red?style=for-the-badge" alt="Estado Archivado"/>
    <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js"/>
    <img src="https://img.shields.io/badge/discord.js-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="discord.js"/>
    <img src="https://img.shields.io/badge/Lavalink%20%2F%20Poru-Audio-FF5722?style=for-the-badge&logo=lavalink&logoColor=white" alt="Lavalink Poru"/>
    <img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB"/>
  </p>

  <p>
    <strong>Bot de Discord impulsado por Lavalink y Poru para ofrecer reproducción de audio de alta fidelidad, control de colas y soporte multiplataforma.</strong>
  </p>
</div>

---

> [!IMPORTANT]
> Este repositorio ha sido **archivado** y se encuentra en modo de solo lectura. Ya no recibe mantenimiento, actualizaciones ni soporte activo.

## Características

* **Audio de alta calidad:** Integración directa con nodos de **Lavalink** mediante **Poru** para streaming estable y de baja latencia en canales de voz.
* **Soporte multiplataforma:** Reproducción directa desde fuentes como YouTube y SoundCloud.
* **Comandos Slash dedicados:** Arquitectura organizada para ejecutar controles musicales (`play`, `pause`, gestión de colas) directamente desde los comandos de barra de Discord.
* **Persistencia de datos:** Almacenamiento y gestión de configuraciones mediante **MongoDB**.

## Requisitos

* **Node.js:** Versión `18` o superior recomendada.
* **Servidor Lavalink:** Un nodo de Lavalink activo y accesible (local o remoto) con su host, puerto y contraseña configurados.
* **Base de datos MongoDB:** Una instancia local o en la nube (MongoDB Atlas).
* **Aplicación de Discord:** Un bot creado en el [Portal de Desarrolladores de Discord](https://discord.com/developers/applications) con permisos para conectarse y hablar en canales de voz.

## Instalación e inicio rápido

1. Clona o descarga este repositorio en tu equipo local:
   ```sh
   git clone [https://github.com/Gh0zd/Bot-Lavalink-Simple.git](https://github.com/Gh0zd/Bot-Lavalink-Simple.git)
   ```
2. Instala las dependencias del proyecto:
   ```sh
   npm install
   ```
3. Configura el token del bot, la URI de MongoDB y las credenciales del nodo de Lavalink dentro de la carpeta `src/config/` (o en tu archivo `.env` según corresponda).
4. Inicia el bot:
   ```sh
   npm start
   ```

> [!NOTE]
> Asegúrate de que tu nodo de **Lavalink** esté iniciado y operativo antes de encender el bot para evitar errores de conexión en los eventos de Poru.

## Estructura del proyecto

```text
.
├── src/
│   ├── All_Files/             # Recursos 
│   ├── commands/
│   │   └── slash/
│   │       └── music/         # Comandos de barra (/) para control musical
│   ├── config/                # Archivos de configuración, tokens y nodos Lavalink
│   ├── events/                # Eventos generales del cliente de Discord
│   ├── functions/             # Funciones auxiliares y utilidades internas
│   ├── handlers/              # Cargadores dinámicos de comandos y eventos
│   ├── poruEvents/            # Eventos de reproducción, colas y conexión de Lavalink
│   └── index.js               # Punto de entrada principal del bot
├── package.json               # Dependencias y scripts de ejecución
└── README.md                  # Documentación del proyecto
```

## Capturas

<p align="center">
  <img src="https://i.postimg.cc/P5HjqwSD/image.jpg" alt="Vista previa del bot de música en Discord" width="80%" />
</p>
