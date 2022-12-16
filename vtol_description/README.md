# Descripción URDF

Para visualizar el modelo del balancín ejecutar:

```
roslaunch vtol_description vtol_rviz.launch gui:=true
```

## Contenido

### Archivos de lanzamiento
El directorio `launch` contiene los siguientes archivos de lanzamiento:

 * `vtol_rviz.launch`: carga la descripción del balancín y lanza RViz para su visualización. Con el argumento `gui` a `true` se pueden controlar las uniones del modelo.

### Archivos de descripción
El directorio `urdf` contiene los siguientes archivos de descripción del balancín:

 * `ciii_vtol.xacro`: archivo de descripción general (incluye los demás archivos).
 * `params.xacro`: parámetros del modelo (dimensiones, volumen, masa, etc.).
 * `motor.xacro`: macro de descripción de los motores.
 * `propeller.xacro`: macro de descripción de los propulsores.
 * `lateral.xacro`: macro de descripción de los laterales de la base del balancín.
 * `material.xacro`: descripción del material para la visualización en RViz.
 * `ciii_vtol.gazebo`: plugin de propulsores, plugin de `ros_control` y material para el simulador Gazebo.
