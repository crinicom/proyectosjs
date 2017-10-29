# proyectosjs
Sistema en js
Me parece que tengo dos opciones: METEOR, que lo veo muy encapsulado, o SAILS.JS, que lo entiendo mejor
https://scotch.io/tutorials/build-a-sailsjs-app-from-api-to-authentication
me parece que voy por Sails, que maneja el tema de usuarios en forma nativa.

Empiezo a pensar en lo que voy a necesitar para mi app.
Voy a pensar en la estructura y las funcionalidades, aunque sea en forma desordenada, porque las funcionalidades dan forma a la db por ejemplo.

LO BASICO
_Project Charter_
Un formulario para cargar la información básica del Proyecto:
Título del proyecto
SponsorS (personas)
FU esperable: que cuado tipee parte del nombre me sugiera gente en la DB
Contexto y aclance
Antecedentes
ObjetivoS <- ver qué valor tiene mostrarlos a lo largo del desarrollo
Equipo de trabajo: personas <-- ver accesibilidad al proyecto a través de esto
InvitadoS <- por temas de accesibilidad
Hitos de Proyecto: hito+fecha <- FU esp: la gantt debe tener estos hitos identificados

_EDT_
Ideal que me permita generar el arbol a partir de los OBJETIVOS
FASE I: que por lo menos ponga los OBJETIVOS como titulo y me permita ingresar tareas asociados a cada una. ASOCIACION TAREA A-B-C-OBJETIVO. Siempre en formato simple, podría permitirme determinar que una tarea que cargué "requiere detalle" entonces la plantea como un subtitulo indentado estilo lista, y me agrega campos de ingreso abajo.
FU esperable: que me sugiera actividades relacionadas a OBJETIVOS. Diseñar-construir-validar en general

Tarea |
--- |
Tipo
ID  
Texto
Fecha_crea
Creado_por
Asignado_a *
Hereda_de
Asociado_a {tipo_obj + id}


-STAKEHOLDERS-
Me permite pensar los stk y plan de comunicaciòn a partir de la lista de TAREAS (en principio)
Trae a los sponsors al principio

STAKEHOLDER |
--- |
Tipo
ID  
Nombre
Plan_comm
Objeto_comm
Fecha_crea
Creado_por
Asignado_a *
Asociado_a {tipo_obj + id}

-RIESGOS-
Me permite pensar los riesgos y plan de mitigación a partir de la lista de STK (en principio)

RIESGO |
--- |
Tipo
ID  
Descripcion
Impacto
Plan_mitigacion
Fecha_crea
Creado_por
Asignado_a *
Asociado_a {tipo_obj + id}

REVISANDO LO QUE ESCRIBI: tendrá sentido ASIGNAR A los planes de comunicación, mitigacion, etc o mejor creo un ITEM_GANTT que tenga asociación con la parte operativa de las otras áreas de conocimiento?
De esa manera lo que se ASIGNA_A es el item gantt, que se -relaciona- con cualquiera de los anteriores.
De esta manera tngo flexibilidad para crear items gantt que no asocian a nada.
Tengo que evaluar los eventos upd y del asociados a stk/risk/task para hacer el binding con los items de la Gantt


# MANEJAR USUARIOS
https://medium.com/of-all-things-tech-progress/starting-with-authentication-a-tutorial-with-node-js-and-mongodb-25d524ca0359

este muestra hasta la pagina de profile https://www.sitepoint.com/user-authentication-mean-stack/


# CREAR LA DB
# apis
https://www.codementor.io/olatundegaruba/nodejs-restful-apis-in-10-minutes-q0sgsfhbd
# testing
# capa ui
# multiusuario
http://dreamerslab.com/blog/en/write-a-todo-list-with-express-and-mongodb/

