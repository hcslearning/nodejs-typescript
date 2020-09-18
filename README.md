# nodejs-typescript

1. Crear carpeta para proyecto e iniciar con npm init
```bash 
mkdir mi-proyecto && cd mi-proyecto
npm init -y 
```

2. Instalar typescript globalmente si no se ha hecho 

```bash 
$ sudo npm install -g typescript 
```

3. Iniciar el archivo de configuración de Typescript y adecuar según sea necesario
```bash
$ tsc --init
```

4. Opcionalmente agregar a .gitignore el directorio outputDir del código generado por Typescript 

5. Agregar configuración para ejecución en package.json
```json 
{
  "name": "nodejs-typescript",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "start": "tsc && node dist/index.js",
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "author": "",
  "license": "ISC",
  "devDependencies": {
    "typescript": "^4.0.2"
  },
  "dependencies": {
    "@types/node": "^14.11.1"
  }
}
```

