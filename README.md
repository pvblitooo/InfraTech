# Portal de Gestión de Incidentes - InfraTech S.A.
## Este ReadMe describe la estructura y organisación del directorio del frontend para la aplicación de gestión de incidentes. El frontend está desarroyado utilisando el framework Angular.

# Directorio
Frontend------¡ 

              node_modules 
              
              public
              
              src------------¡
              
                             app-------------¡
                             
                                             incident-form
                                             
                                             incident-list
                                             
                                             statics-board
                                             
                             models----------¡
                             
                                             incident.ts
                                             
                             services--------¡
                             
                                             incident.spec.ts
                                             
                                             incident.ts
                                             
                             app.config.ts
                             
                             app.html
                             
                             app.routes.ts
                             
                             app.scss
                             
                             app.spec.ts
                             
                             app.ts
                             
              index.html
              
              main.ts
              
              styles.scss
              

              

## Ejecución Local
1. Clonar repositorio: `git clone https://github.com/pvblitooo/InfraTech.git`
2. Instalar dependencias: `npm install`
3. Iniciar servidor: `ng serve`

## Ejecución con Docker
1. Construir imagen: `docker build -t infratech-frontend .`
2. Ejecutar contenedor: `docker run -p 80:80 infratech-frontend`

## Estructura Generall del Directorio (/frontend)

A continuasión, se detalla el propósito de las principales carpetas y archivos en la raíz del directorio frontend:

node_modules/: Contiene todas las dependencias y paketes de Node.js requeridos por el proyekto. Administrado por npm o Yarn.

public/: Almasena activos estáticos que se sirven directamente, como imájenes, fuentes o archivos de konfigurasión global.

src/: Es el corasón de la aplicación Angular, conteniendo todo el código fuente.

.editorconfig: Archivo de configuración para mantener estilos de codificación consistentes entre diferentes editores e IDEs.

.gitignore: Especifca los archivos y carpetas que Git debe ignorar.

angular.json: Archivo de configuración del CLI de Angular. Define la estructura del proyecto, builds, y otras configuraciones específicas de Angular.

package-lock.json: Registra las versiones exactas de cada dependencia instalada.

package.json: Define los metadatos del proyecto, scripts (como start, build, test), y dependencias.

README.md: Este mismo archivo, proporcionando información sobre el proyecto.

tsconfig.app.json: Configuración específica de TypeScript para la compilación de la aplicación Angular.

Detalles de la Carpeta src/


## La carpeta src contiene los siguientes elementos fundamentales:

app/: Contiene los módulos, componentes, servisios y modelos que conforman la lógica y la interfaz de usuario de la aplicación.

components/: Subdirectorio que agrupa componentes reutilizables de la interfaz de usuario.

incident-form/: Componente para el formulario de creación/edición de incidentes.

incident-list/: Componente para listar los incidentes.

statistics-board/: Componente para mostrar estadísticas relacionadas con los incidentes.

models/: Define las estructuras de datos o modelos utilizados en la aplicación.

incident.ts: Modelo TypeScript para representar un incidente.

services/: Contiene los servicios de Angular, responsables de la lógica de negocio, acceso a datos (APIs), etc. Se infiere la existencia de incident.service.ts
para gestionar las operaciones CRUD de incidentes.

app.config.ts: Configuración a nivel de aplicación, introducida en versiones más recientes de Angular para configuraciones de bootstrapApplication.

app.html (asumido app.component.html): Plantilla HTML para el componente raíz de la aplicación (AppComponent).

app.routes.ts: Define las rutas de navegación de la aplicación.

app.scss (asumido app.component.scss): Estilos SCSS específicos para el componente raíz (AppComponent).

app.spec.ts (asumido app.component.spec.ts): Pruebas unitarias para el componente raíz (AppComponent).

app.ts (asumido app.component.ts): Lógica TypeScript para el componente raíz de la aplicación (AppComponent).

index.html: El archivo HTML principal que se carga en el navegador. Angular inyecta la aplicación aquí.

main.ts: El punto de entrada principal de la aplicación. Responsable de arrancar el módulo raíz de Angular (o la aplicación standalone).

styles.scss: Archivo para los estilos globales de la aplicación utilizando SCSS.
