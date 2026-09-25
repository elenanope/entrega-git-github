## Actividad de Git y Github
Esta es una actividad para asimilar el uso de un repositorio a través de Git y con la ayuda de Github

## Problemas y dudas
No sabía si al clonar el repositorio, este se enlazaría a la carpeta en la que estabas al realizar esta acción. Al clonarlo me ha confundido la manera en la que visual studio code representaba la nueva carpeta, pero al crear archivos de prueba a su misma altura, he comprobado que efectivamente la carpeta del repositorio se había creado donde debería

## Historial de la práctica
<ol>
<li><b>Historial primer commit:</b>
<ul><li>9fbe88d (HEAD -> main) Crear estructura inicial del proyecto</li></ul>
</li>
<br>
<li><b>Historial de feature/contacto:</b> se ha creado la rama feature/contacto, se le ha añadido la página de contacto y se ha commiteado.
<p>
<ul>
<li>6b4479f (HEAD -> feature/contacto) Añadir página de contacto</li>
<li>22f11a4 (origin/main, main) Añadido información e historial al README</li>
<li>9fbe88d Crear estructura inicial del proyecto</li>
</ul>
</li>
</p>
<br>

<li><b>Historial después del merge:</b> volviendo a main, he mergeado la rama feature/contacto a main para tener el último commit que solo estaba en esa segunda rama.
<p>
<ul>
<li>6b4479f (HEAD -> main, origin/feature/contacto, feature/contacto) Añadir página de contacto</li>
<li>22f11a4 (origin/main) Añadido información e historial al README</li>
<li>9fbe88d Crear estructura inicial del proyecto</li>
</ul>
</li>
</p>

<br>

<li><b>Historial después de actualizar desde GitHub:</b> he añadido una foto a través de la web de GitHub y tras comprobar (con git status después de hacer un fetch) que en el local tenemos un commit pendiente de pullear (para estar actualizados), hago git pull y ya aparece el siguiente log.
<p>
<ul>
<li>7451ec1 (HEAD -> main, origin/main, origin/HEAD) Añadir imagen pato en remoto</li>
<li>6b4479f (origin/feature/contacto, feature/contacto) Añadir página de contacto</li>
<li>22f11a4 Añadido información e historial al README</li>
<li>9fbe88d Crear estructura inicial del proyecto</li>
</ul>
</li>
</p>

<br>

<li><b>Historial de feature/contacto después de incorporar la rama principal:</b> al haber hecho pull desde main, el último commit no está actualizado en la rama feature/contacto, así que al cambiarnos a ella, mergeamos main a esta otra para tener la misma información.
<p>
<ul>
<li>7451ec1 (HEAD -> feature/contacto, origin/main, origin/HEAD, main) Añadir imagen pato en remoto</li>
<li>6b4479f (origin/feature/contacto) Añadir página de contacto</li>
<li>22f11a4 Añadido información e historial al README</li>
<li>9fbe88d Crear estructura inicial del proyecto</li>
</ul>
</li>
</ol>
</p>

## Observaciones
<ul>
<li>Cada vez que hagas un commit en una <b>rama</b> nueva, al pushear a remoto debes especificar su nombre (por ejemplo: <i> git push --set-upstream origin feature/help-page</i>), en vez de solamente git <b>push</b></li>
<br>
<li>
Al hacer <b>commits</b>, se debe usar una buena nomenclatura, que sea comprensible y descriptiva, aunque lo más resumida posible. Si un compañero observa nuestros commits deberían de ser capaces de entenderlos (al menos en general).
</li>
<br>
<li>
Al hacer <b>merge</b> debes estar en la rama que está desactualizada y mergear la que tenga los commits (/cambios) que te faltan.
</li>
<br>
<li>
Cuando haces <b>fetch</b>, tu local se actualiza, para saber si le falta algún commit del remoto. Si encuentra commits por descargar y estás listo, los podrás descargar en tu local haciendo git <b>pull</b>.
</li>
<br>
<li>
Si has hecho algún cambio <b>directamente desde GitHub </b>, deberás actualizar tu local, ya que solo existirán en el remoto y no en tu local. Para actualizarlos tendrás que hacer <b>fetch</b> y <b>pull</b>, al hacer eso obtendrás todos los cambios no actualizados del remoto al local.
</li>