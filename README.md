- Name: Joan Camilo Betancourt Gonzalez

- Graphical representation of the system structure: Mirar ![System Structure.drawio.png](https://github.com/CamiloBetancourtg/Swarch/blob/549969657687268e13b93b4828bea844d7f9ab90/System%20Structure.drawio.png)

- 5 system properties:

    1. El sistema de registro de notas se muestra a través de diferentes capas, primero de los modelos (manejo de base de datos), despues hacia los servicios (logica de negocio) y despues hasta las templates y controladores (vista del sistema).

    2. El sistema tiene facilidad de mantenibilidad, ya que el acceso a datos esta separado en repositorios y la logica de notas en servicios, haciendo que sea de facil refactorización y extensión.

    3. Al usar contenedores de docker, el sistema puede ser ejecutado en cualquier sistema operativo y funciona igualmente.

    4. Los datos ingresados al sistema pasan por un proceso secuencial, de forma que atraviesa diferentes controles antes de llegar a la base de datos.

    5. Gracias a la orquestación de docker, el sistema contiene todo el despliegue en un unico comando donde se ejecuta la base de datos y la aplicación.


Para ejecutar el sistema, ponga en consola:
- docker-compose up --build, esto correra el contenedor y el servidor para conectarse localmente. 