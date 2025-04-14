
Sistema de relevamiento al contribuyente (SIRECO). Es una pagina web simple desarrollada en html, css, javascript y mysql. Se puede realizar una busqueda en la base de datos por medio del dni y completar el formulario con los datos del contribuyente en caso de que aun no fue cargado para que queden guardados en la base de datos. Junto a sus datos se puede guardar de forma relacionada, el/los inmuebles, rodados (auto y moto) o comercios que éste posea. El sistema se encuentra dockerizado, listo para correr el comando docker compose up.

/* Arbol del proyecto
SIRECO/     Sistema de Relevamiento del Contribuyente.
├── sireco_back/
│   ├── node_modules/
│   ├── src/
│   │   ├── controller/
│   │   |    └── autController.js
│   │   ├── db/
│   │   |    └── config.js
│   │   └── routes/
│   │        └── router.js
│   |
│   ├── .env     # Variables de entorno.
│   ├── app.js
│   ├── Dockerfile
│   ├── package-lock.josn
│   └── package.json
│ 
├── sireco_fron/
│   ├── css/           	 # Estilos de las paginas.
│   │   ├── checkBox.css
│   │   ├── checkRod.css
│   │   ├── constrib.css
│   │   └── index.css
│   │
│   ├── js/                # Logica de la pagina
│   │   ├── checkCement.js
│   │   ├── checkComer.js
│   │   ├── checklnm.js
│   │   ├── checkRod.js
│   │   ├── index.js
│   │   └── localidad.js
│   │
│   ├── checkCement.html
│   ├── checkComer.html
│   ├── checklnm.html
│   ├── checkRod.html
│   ├── contrib.html
│   ├── dockerfile
│   ├── index.html
│   ├── localidad.html
│   └── sireco.conf 
│       
├── .gitignore         # Ignora archivos innecesarios en el repositorio
├── docker-compose.yml         # Archivo de configuracion de docker.
├── init.sql         # Archivo de inicializacion de la base de datos.
└── README.md          # Documentación del proyecto
