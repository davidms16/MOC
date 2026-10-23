# Reflexion — MiniApp de Tareas

**Nombre:** David Menéndez Santos

## 1. Diferencia GET y POST, con un ejemplo de tu código donde usarías cada uno.

con get los datos se ven en la url mientras que con post no. getMessage y method="POST"

## 2. ¿Qué es una cabecera HTTP? Pon un ejemplo de cabecera de petición y otro de respuesta que hayas visto hoy.

las cabeceras muestran informacion sobre la peticion. un ejemplo de peticion seria Host: localhost:8080 y uno de respuesta seria Location: /index.php

## 3. Explica con tus palabras qué es una cookie a nivel técnico: dónde se guarda, cómo viaja y quién puede leerla.

es un pequeño archivo, de texto, que una web guarda en el ordenador para recordar datos. se guarda en el propio dispositivo, en una carpeta controlada por el navegador que la genero. viaja a traves de las cabeceras precisamente. solo la puede leer la web que la genero originalmente

## 4. Explica con tus palabras qué es una sesión y en qué se diferencia de una cookie. ¿Dónde se guarda cada una?

las cookies se guardan en el dispositivo del usuario, mientras que las sesiones se guardan en el servidor. la seguridad de la cookie, debido a que se guarda en el mismo dispositivo, es baja, al contrario que la de la sesion, ya que se guarda en un lugar inaccesible para el usuario. a su vez, las sesiones guardan mas datos que las cookies, por lo que suelen servir para guardar formatos de pago, sesiones de una web iniciadas o datos utiles para la web, mientras que las cookies guardan preferencias de idioma y similar

## 5. Cita los tres mecanismos de persistencia usados en la MiniApp y para qué sirve cada uno.

_(sin responder)_

## 6. Diferencia autenticación vs autorización con un ejemplo de tu código.

la autenticacion confirma que la persona que intenta entrar eres tu, mientras que autorizacion verifica lo que puedes hacer y lo que no.

## 7. ¿Por qué llamamos a session_regenerate_id(true) tras el login?

para evitar un ataque informatico

## 8. ¿Qué pasaría si un usuario edita su cookie PHPSESSID a otro valor? ¿Y si edita ultimo_email?

en el primer caso se le crearia una sesion vacia en el caso de que añada datos inventados debido a que no encontraria credenciales con los datos editados. en el caso del ultimo_email el usuario podria llegar a suplementar una identidad con un rol superior

## 9. ¿Qué significa que PHPSESSID tenga HttpOnly? ¿Qué ataque mitiga?

esto hace que ningun script de javascript puda ejecutarse si se cambia el valor de la cookie. prevee ataques de secuestro de sesion
