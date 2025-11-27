# Gestor de Notas con MongoDB

## Capturas de Pantalla

### Vista Principal
<img width="1474" height="887" alt="image" src="https://github.com/user-attachments/assets/925e307a-8b5e-4001-99f7-3197d9765403" />

### Crear/Editar Nota
<img width="1479" height="857" alt="image" src="https://github.com/user-attachments/assets/e9c229c8-d0bf-4e46-9427-50f97c2c47f4" />
<img width="1481" height="853" alt="image" src="https://github.com/user-attachments/assets/9fb98439-2076-40a6-a266-6d8f127735a6" />
<img width="1479" height="849" alt="image" src="https://github.com/user-attachments/assets/d638a0da-4490-47c4-9550-08bbe0c2c6f3" />
<img width="1480" height="848" alt="image" src="https://github.com/user-attachments/assets/c7295ae4-3a28-4a7f-b259-5bc9139844a9" />

### MongoDB
<img width="1647" height="772" alt="image" src="https://github.com/user-attachments/assets/48d10735-f1dd-4b82-97e8-00ed2f824c98" />

## Instalación

### 1️- Clonar el Repositorio

```bash
git clone https://github.com/23300764/MONGO-DB.git
cd GestorNotas_MongoDB
```

### 2- Configurar MongoDB

- Entra a la pagina: https://cloud.mongodb.com/ y crea una cuenta gratis.
- Crea un nuevo cluster:
- Selecciona el tipo gratis que se llama M0
- Dale a crear
- Crea un usuario para la base de datos:
- Ve a donde dice "Database Access"
- Pulsa en "Add New Database User"
- Guarda bien el usuario y contraseña que pongas
- Para conectar con C#:
- Ve a "Database"
- Luego a "Clusters"
- Ahi veras tu base de datos
- Consigue tu cadena de conexion:
- Pulsa el boton "Connect"
- Elige "MongoDB for VS Code"
- Copia el texto que te aparece
- Cambia la parte donde dice tu usuario y tu contraseña por los que creaste
- Este texto lo vas a usar en el siguiente paso

### 3️- Configurar la Aplicación

#### Crear Archivo de JSON en ejectuble

1. Abre la carpeta en donde aparecen los paquetes de nuget y el .exe del form
2. Agrega ahí un archivo nombrado como "appsettings.json" 
3. Escribe en el archivo el json que esta a continuación pero reemplazando la ConnectionString por la tuya 

**Para MongoDB:**
```json
{
 "MongoDB": {
  "ConnectionString": "mongodb+srv://tuusuario:tupassword@cluster0.xxxxx.mongodb.net/",
  "DatabaseName": "GestorNotas",
  "CollectionName": "Notas"
  }
}
```

> Reemplaza `tuusuario`, `tupassword` y `cluster0.xxxxx` con tus credenciales reales de MongoDB Atlas
