# Aprender en tiempos de IA

Estos son los ejercicios de la charla. Son tres:

1. **Leer más código:** le pedimos una app a la IA, anotamos qué queremos que tenga y qué pensamos que va a hacer, lo buscamos en el código y después lo comparamos con la app funcionando.
2. **Escribir más código:** rehacemos esa misma app, primero usando completions y después a mano.
3. **Conseguir un cliente:** buscamos un negocio cerca, le armamos una demo y se la mostramos.

Usá la tecnología que ya conozcas y hacelos a tu ritmo.

[Slides de la charla](https://www.figma.com/slides/u9hMhTKBKHKe04UqdW20xq) · [Video con los ejercicios](https://www.youtube.com/watch?v=UoRvcQ9avgw)

## Ejercicio 1: Leer más código

Cada vez escribimos menos código y leemos más el que escribe la IA. Pero leer código no es mirarlo por arriba y decir «parece que anda». Es poder mirar algo que hace la app y encontrar el código que lo hace.

Para practicarlo, vamos a pedirle una app a la IA. Antes de probarla, vamos a anotar qué queremos y qué pensamos que va a pasar, vamos a leer el código y recién después vamos a comparar nuestras notas con la app funcionando.

1. **Pedile a una IA una app sencilla.** Puede ser una lista de tareas o de supermercado, en v0, Claude, ChatGPT o la que quieras. El prompt no tiene que ser largo: «Hacé una lista de supermercado sencilla y fácil de usar, con todo el código en un solo archivo».
2. **Mientras la IA trabaja, armá tu lista.** Abrí un bloc de notas y anotá qué cosas pensás que tiene que tener (o no tener) la app para ser sencilla y fácil de usar. Me dirán: «es una lista de supermercado, ¿cuántas cosas puede tener?». Bueno, algunos ejemplos:
   - Cuando entro, ¿el foco ya está en el campo para escribir?
   - ¿Puedo agregar apretando Enter?
   - ¿Me deja agregar un producto vacío?
   - ¿Puedo editar o borrar un producto?
   - ¿Puedo ver cuántos me faltan comprar?

   Vos decidís cuáles importan para tu app y cuáles agregar. Todavía no abras el navegador ni la vista previa.
3. **Cuando termine, andá al código, no al navegador.** Buscá cada cosa de tu lista y anotá si está implementada, en qué parte del código y qué pensás que va a pasar cuando uses la app. Si algo no lo entendés, primero intentá razonarlo vos. Si no sale, pedile una pista a la IA.
4. **Leé el resto del código.** Lo que no estaba en tu lista, ¿qué hace? ¿Por qué está ahí? ¿Es una funcionalidad que no necesitás? Anotalo también.
5. **Ahora sí, abrí la app en el navegador.** Compará tus notas con lo que hace la app de verdad. Si algo no coincide, volvé al código hasta entender por qué.
6. **Iterá hasta que quede simple.** Pedile a la IA que saque o cambie lo que sobra o está mal, y cada cambio leelo y probalo de nuevo. La idea es terminar con una app chica y fácil de usar, solo con lo que vos considerás básico.

### Un ejemplo

Pensemos en el foco al abrir la app. Seguramente tenga que ver con el input, así que vamos a buscarlo. En React, si el input tiene `autoFocus`, recibe el foco cuando se monta. Check:

```jsx
<label>
  Producto
  <input name="producto" autoFocus required />
</label>
```

Ojo, eso no significa que el foco vuelva al campo después de agregar un producto. Eso es otra cosa, y también la tenés que buscar en el código y probar.

**La meta:** no solo leer el código de la IA, sino evaluarlo contra lo que esperabas e iterarlo hasta llegar a lo que querías.

## Ejercicio 2: Escribir más código

Casi todo lo que sabemos no lo aprendimos haciendo un curso o viendo un tutorial, lo aprendimos escribiendo código. Mientras más código escribimos, más lo razonamos. Mientras más falla, más formas aprendemos de que no falle. Y eso nos queda.

No se trata de escribir código como fin, sino como forma de aprender, para después entender mejor el código que leemos. Sería tonto no aprovechar lo que nos da la IA, pero si dejamos que lo escriba todo, no lo aprendemos.

Así que vamos a hacer la misma app del ejercicio 1 dos veces más. Sí, tres veces la misma app, cada vez en un proyecto nuevo y desde cero.

### Parte 1: Con completions

1. **Creá un proyecto nuevo, desde cero.** No uses la carpeta del proyecto anterior.
2. **Hacé la misma app,** la versión ya iterada, con lo que consideraste esencial en el ejercicio 1.
3. **Escribila vos, con completions.** O sea, con las sugerencias que te aparecen en el editor mientras escribís (Copilot, Cursor o el que uses). Hay una sola regla: el 100% del código lo escribís vos o el autocomplete mientras escribís. No vale copiar y pegar código de ningún lado ni pedirle a una IA que lo escriba por vos.
4. **Probala con tu lista.** Si te trabás mucho en alguna parte, dejala, seguí con otra cosa y volvé después. Si necesitás mirar cómo estaba hecho en el proyecto anterior, miralo como referencia, pero intentá evitarlo.

### Parte 2: Sin ayuda

1. **Creá otro proyecto nuevo, desde cero.**
2. **Hacé la misma app otra vez,** pero ahora apagá las completions y escribí vos el 100% del código. Podés leer documentación y usar las ayudas de sintaxis normales del editor.
3. **Probala con tu lista y compará las tres versiones.** Fijate qué cosas podés explicar ahora que antes no entendías.

### Por qué tres veces la misma app

Cuando hacemos una app desde cero, en realidad hacemos dos cosas: pensar qué tiene que hacer y descubrir cómo implementarla. Muchas veces creemos que lo tenemos claro, pero cuando empezamos a escribir aparecen dudas y cambios, nos mareamos y nos frustramos.

- **La primera vez** la hizo la IA y vos la iteraste. Ya sabés qué tiene que hacer y hasta la podés usar.
- **La segunda vez** no hay idas y vueltas sobre qué hacer. Tu cabeza se puede enfocar solo en implementarla. Seguro aparezcan algunos problemas, pero no deberían ser grandes.
- **La tercera vez** vas a tener casi todo el código en la cabeza. Vas a estar replicando algo que ya hiciste, pero esta vez solo.

Además, es una app simple y sin sentido. No hay presión por terminarla ni por hacerla rápido, así que no hace falta la IA. El único fin es aprender escribiendo código.

Cuando leíste el código de la IA, habrás pensado «esto lo escribió para tal cosa» o «¿y por qué hizo esto?». Cuando la escribas vos, te vas a acordar de ese código y vas a decir «ah, era por esto». O vas a pensar que sobra, lo vas a sacar, no va a andar y ahí vas a entender para qué servía.

Ese es el momento en el que aprendés algo que te queda, y que posiblemente no hubieras aprendido solo leyendo el código.

**La meta:** escribir código no para escribirlo, sino para aprender, y así entender mejor el código que leés.

> ¿Querés otra vuelta? Hacé que cargar, agregar y borrar tarden un segundo. Pensá qué debería ver la persona mientras espera y qué pasa si hace otra cosa mientras tanto. Después hacé los dos ejercicios otra vez con ese cambio. Y cada tanto, repetilo con apps más complejas: un listado de usuarios, un carrito, un ecommerce.

## Ejercicio 3: Conseguir un cliente

En una entrevista no importa cuántas pokédex o apps de películas tengas. Ninguna app de portfolio le gana a la experiencia con clientes reales.

Antes, vivir de hacer desarrollos propios o para clientes era un salto de fe. Hoy podemos armar algo mucho más rápido, sin dejar de lado todo lo demás, y empezar a ganar experiencia desde otro lado.

Así que la tarea es conseguir un cliente. Posiblemente gratis, pero no importa, porque le vas a dedicar muy poco tiempo. En vez de hacer un curso o mirar una serie una tarde, vas a hacer una app para un cliente, y te va a servir mucho más.

Acá sí podés usar la IA para hacer el prototipo rápido. No quiero que inviertas mucho tiempo ni esfuerzo en el desarrollo, porque la meta es otra.

### Qué tipo de app

Buscá ideas que sean simples en tres sentidos: **poco código, poco tiempo de desarrollo y poco esfuerzo para que el cliente la empiece a usar**. No tenemos que cambiarle la forma de trabajar al cliente. Si la app te lleva dos horas pero el negocio tiene que cambiar toda su forma de trabajar, posiblemente no sea una buena primera propuesta.

Algunos ejemplos de la charla:

- **Una cafetería:** un mapa muestra la zona donde hay 10 códigos escondidos cerca del local. Quien encuentra uno lo canjea por un café gratis y el código desaparece del mapa. A la cafetería le cuesta 10 cafés, y a cambio puede hacer un reel y atraer gente al local.
- **Una heladería:** quien compra un helado puede llevárselo gratis si gana un juego. Tiene que memorizar dónde están 12 tachos de helado y después adivinar dónde están 3 de ellos. Puede haber hasta 10 ganadores.

En estos casos hay muy pocos datos sensibles o formas de abusar de la app, así que revisar el código lleva poco tiempo. Tenelo en cuenta para lograr un buen balance entre resultado y esfuerzo, más si el trabajo es gratis.

### Qué vas a hacer

1. **Encontrá algo concreto para resolver** en un negocio o emprendimiento que frecuentes o tengas cerca. Además de los ejemplos de arriba, puede ser una carta por QR, un catálogo para armar pedidos o una agenda de actividades. Pensá también quién va a actualizar la información y cuánto trabajo le va a dar.
2. **Armá una demo chica.** Que resuelva una sola cosa y que la puedas mostrar en pocos minutos. Usá datos de ejemplo y no le agregues funcionalidades antes de saber si le interesan.
3. **Mostrala y escuchá.** Andá con algo que ya funcione, contale qué pensaste y preguntale si le serviría. Si le interesa, acuerden una prueba chica: qué incluye, qué tiene que aportar el negocio y cuánto va a costar, aunque esta primera vez sea gratis.

Podés arrancar la conversación así:

> Hola, estoy practicando desarrollo y armé esta demo pensando en tu negocio. Vi que [observación] y se me ocurrió [solución]. ¿Te la muestro y me decís si te sirve?

Hacé que probarla sea fácil: mandar un link o poner un QR es mucho menos trabajo que capacitar a todo el equipo o cargar cientos de productos. Si funciona, después hay tiempo para hacerla crecer.

**La meta:** resolverle algo útil a una persona real y aprender de lo que te diga. La demo abre la conversación, pero el cliente aparece cuando alguien acepta trabajar con vos.
