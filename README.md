Fecha entrega: Lunes 16.
En un nuevo repositorio (todo-app):

1. Crear un layout para una app de tareas con estilo de mobile first dejando en la parte inferior siempre visible un menu 3 botones (Pendientes, Todas, Perfil). Toda la App estará creada en un único archivo HTML.


2. Crear un header con estilos a tu gusto.

3. En base al sistema de tareas simples hecho en casa, convertir las tareas en objetos agregando un id a cada una.

4. Agregar una nueva opción de "isCompletada" booleana para indicar si esta completada o no.

5.  Agregar un checkbox y un botón a cada item de la lista para marcarla como completa/incompleta

6. Agregar un botón de eliminar tarea a cada tarea.

7. Crear las funciones y métodos para cada botón.


7.1. 
```js  
    //Metodo 1: forEach + splice
      listaDeTareas.forEach((tarea, index) => {
        if(tarea.id == idTarea){
          listaDeTareas.splice(index,1);
        }
      });

      //Metodo 2: findIndex
      const index = listaDeTareas.findIndex( tarea => tarea.id == idTarea);
      listaDeTareas.splice(index,1);
      mostrarTareas();
    

    // Metodo 3: usando Filter (recuerda que cambiamos de const a let en listaDeTareas)
    listaDeTareas = listaDeTareas.filter(tarea => tarea.id != idTarea);

```
8. Menu: implementar lo visto en clase de Tabs para el menu

9. Perfil: implementar lo visto en clase de Acordeón para crear un Perfil

10. En Pendientes solo mostrar la lista de tareas sin hacer, y en Todas mostrar ambas, completadas y no completadas.