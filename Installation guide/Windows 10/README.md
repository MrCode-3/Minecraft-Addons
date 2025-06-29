
# 👩‍💻 Instalación de addons - Windows 10

En esta guía enseñaremos paso a paso la instalación de addons en un servidor, usando el Host [EasyMinecraftHosting](https://easyminecrafthosting.com/), desde Windows 10.

![EasyMinecraftHosting](https://github.com/MrCode-3/Minecraft-Addons/blob/main/resources/EasyMinecraftHosting.png)

## ❗❗ Cosas a tener en cuenta
- No uses addons o cualquier otro pack que provenga de la Marketplace ya que no funcionarán en servidores que no sean realms.
- Si después de seguir esta guía paso a paso uno o varios de tus addons no funcionan correctamente puede deberse a uno de estos problemas:
  - Algunos addons necesitan ir instalados en un orden espécifico para poder funcionar correctamente.
  - Es probable que exista una incompatibilidad entre los addons.
  - No es compatible con la versión de minecraft de tu servidor.
  - El addon no funciona debido a un error en su código.
- Aunque esta guía fue probada en Windows 10 puede funcionar tambien en Windows 11 pero es posible que algún paso mostrado aqui se tenga que ejecutar de manera diferente.

## Método 1 - Mundo desde cero
###  💡 Pasos Previos
- Desde Minecraft crea un mundo e instala los addons o texturas que desees. Como ejemplo usaremos el addon **Better on Bedrock**

 ![ResourcePack](https://github.com/MrCode-3/Minecraft-Addons/blob/main/resources/Windows-rp-install.png)

 ![BehaviorPack](https://github.com/MrCode-3/Minecraft-Addons/blob/main/resources/Windows-bp-install.png)

- Recuerda activar las `opciones experimentales` necesarias en el caso de que tus addons las necesiten.

 ![Experimentals](https://github.com/MrCode-3/Minecraft-Addons/blob/main/resources/Windows-experimentals.png)

- Haz clic en crear y espera hasta que hayas ingresado a tu mundo, luego de eso abandona la partida y cierra Minecraft.

### 🔎 Localiza los datos de tu mundo
- Presiona la tecla Windows y sin soltar pulsa la tecla R.
- En el programa llamado *Ejecutar* escriba `%appdata%\..\Local\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang` y de clic en el botón Aceptar.

 ![Execute](https://github.com/MrCode-3/Minecraft-Addons/blob/main/resources/execute-program.png)

- Ingresa en la carpeta **minecraftWorlds** y busca la carpeta del mundo que creaste, selecciónala y comprímela en formato zip. Si dentro de la carpeta minecraftWorlds se visualizan muchas otras carpetas y no sabes cual de ellas corresponde a tu mundo revisa la fecha y la hora en que fueron creadas/editadas para poder identificarla.

![World zip](https://github.com/MrCode-3/Minecraft-Addons/blob/main/resources/World-zip-Windows.png)

- Eso creará un archivo que zip que tendrás que subir al servidor.

### 📦 Importación del mundo al servidor
- Apaga el servidor.
- Dirígete a la pestaña **Archivos** del panel de tu servidor, luego ingresa en la carpeta worlds.

![WorldsFolderServer](https://github.com/MrCode-3/Minecraft-Addons/blob/main/resources/Worlds%20Folder%20Server.png)

- Arrastra el archivo comprimido de tu mundo desde tu pc a la carpeta del servidor previamente mencionada.

![UploadWorld](https://github.com/MrCode-3/Minecraft-Addons/blob/main/resources/UploadWorldWindows.png)

- Una vez de que el archivo se haya subido completamente haz clic derecho en el y luego da clic en la opción **Extract**.

![Extract](https://github.com/MrCode-3/Minecraft-Addons/blob/main/resources/ExtractWorldWindows.png)

- Eso hará que se descomprima y aparezca la carpeta de tu mundo, si no aparece prueba recargar la página.
- Copia el nombre de la carpeta de tu mundo, en este ejemplo el mundo se llama **Bo0+Xvn97gk=** pero si deseas puedes renombrarlo con otro nombre. En este caso lo renombraré a **Mi Mundo**.

![ServerWorld](https://github.com/MrCode-3/Minecraft-Addons/blob/main/resources/ServerWorldWindows.png)

![RenameServerWorld](https://github.com/MrCode-3/Minecraft-Addons/blob/main/resources/RenameServerWorldWindows.png)

![NewNameServerWorld](https://github.com/MrCode-3/Minecraft-Addons/blob/main/resources/NewNameServerWorldWindows.png)

### ⚙ Configuración del archivo server.properties
- Necesitarás retroceder a una carpeta anterior donde podrás encontrar el archivo llamado **server.properties**.
- Accede a este archivo y busca la línea donde se haga mención de la opción `level-name`, edita su valor colocando el nombre de la carpeta de tu mundo que en este ejemplo se llama **Mi Mundo**. Ten en cuenta que este apartado es sencible a las mayúsculas y minúsculas asi que coloca el nombre tal cual está en la carpeta de tu mundo.

![server.propertiesLevelName](https://github.com/MrCode-3/Minecraft-Addons/blob/main/resources/serverpropertiesLevelNameWindows.png)

- Da clic en el botón **Guardar Archivo**.
- ¡Ya quedó listo! Finalmente enciende tu servidor y disfruta de tu juego.


