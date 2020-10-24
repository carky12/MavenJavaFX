# Proyecto Maven con JavaFX
Proyecto preconfigurado de JavaFX para Maven. Añadidas librerías para soporte JPA e Hibernate

## Tecnologías 🚀

* Java
* JavaFX
* Hibernate-core
* JPA
* H2/MySQL

## Construcción del proyecto 📖

La estructura de carpetas ya está pre-configurada. En la carpeta main/resources encontramos:
* app: para dejar archivos de recursos de la propia aplicación.
* css: para dejar los archivos de estilos en caso de utilizarlos para el desarrollo de los formularios.
* fxml: para dejar los archivos fxml propios de los formularios de JavaFX (desarrollados con SceneBuilder).
* img: para dejar las imágenes utilizadas en los formularios.

Está añadido el plugin de Maven para realizar la generación. 

			<plugin>
				<groupId>com.zenjava</groupId>
				<artifactId>javafx-maven-plugin</artifactId>
				<version>8.8.3</version>
				<configuration>
					<mainClass>app.AppMain</mainClass>
				</configuration>
			</plugin>
      
Para realizar la generación hacer maven build y guardar las siguientes configuraciones:

* JFX_JAR: goals -> jfx:jar. Se generará el JAR correspondiente al proyecto.
* JFX_NATIVE: goals -> jfx:native. Se generará el autoinstalable correspondiente.
* JFX_RUN: goals -> jfx:run. Se ejecutará el proyecto.

[carky](https://github.com/carky12) 😊
