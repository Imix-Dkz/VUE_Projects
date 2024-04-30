# Curso VUE.js
Este curso se basa en una serie de videos de capacitación y uso de VUE.js partiendo del la lista de reproducción ["Curso VUE Profesional"](https://www.youtube.com/watch?v=vOdj_e3Z4jY&list=PLDllzmccetSNgykILXnHMeuO-y-gRcF-i&index=2), así como algunos otras guias o tutoriales que facilitne información para para aprender y añadir, en el cual se iran añadiendo carpetas, así como notas en este documento que profundicen en los conocimientos adquiridos para hacer desarrollo en VUE...

0. [Contenidos](#contenidos)
1. [Instalación](#instalación)
2. wedfwefwe

# Contenidos
En este apartado se dará un breve resumen de los contenido que se mostrarán en cada directorio y su intención...
Por ejemplo en el directorio "01_Fundamentos", se añadirán pequeños desarrollos partiendo de las siguientes fuentes:
* [VUE en 10 minutos](https://www.youtube.com/watch?v=9AHMihFhrzw)
  + Creación de un proyecto
  + Estructura de directorios/archivos
  + Directivas "v-" , como v-click, v-on, v-model, Eventos ESTANDARD-DOM
    - ![v-on](00_Media\0001_v-on.png) 
  + Algunas directivas ciclicas como "v-for" ó para identificación como ":key"
  + v-bind
  + vuex y propiedades computadas
* [Fundamentos VUE.js +Vite +API](https://www.youtube.com/watch?v=PL-aTHv2L3E&list=PLPl81lqbj-4J-gfAERGDCdOQtVgRhSvIT)
* [Fundamentos PL V1](https://www.youtube.com/watch?v=vOdj_e3Z4jY&list=PLDllzmccetSNgykILXnHMeuO-y-gRcF-i&index=2)
* 

# Instalación
Para el proceso de instalación del framework/CLI se requiere tener un controlador de dependencias, se recomienda "Node.Js", pero tambien pueden usar "Yarn", queda a gusto del desarrollador

```
   npm install -g @vue/cli
   //Se puede verificar si fue correctamente instalado 
   $ vue --version
   @vue/cli 5.0.8
```
Lo siguiente es iniciar un proyecto en VUE, por lo que se usará el siguiente comando:
```
    vue create my-proyect-name
    //En nuestro caso, para comenzar, usaré( NO USAR LETRAS MAYUSCULAS )
    vue create f01-01-vue10min
```