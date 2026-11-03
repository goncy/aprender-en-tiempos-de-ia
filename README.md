# Aprender en tiempos de IA

Estos son los ejercicios de la charla. Son cuatro: uno para aprender a leer el código que escribe la IA, dos para aprender escribiéndolo y uno para llevarle una solución a un cliente real. Usá la tecnología que ya conozcas y hacelos a tu ritmo.

[Slides de la charla](https://www.figma.com/slides/u9hMhTKBKHKe04UqdW20xq) · [Video con los ejercicios](https://www.youtube.com/watch?v=UoRvcQ9avgw)

### Ejercicio 1: Versión solo IA

Vamos a pedirle a una IA que nos haga una app y, antes de probarla, vamos a leer el código para entender qué hace.

1. **Pedile a una IA una app sencilla.** Puede ser una lista de tareas o de supermercado, en v0, Claude, ChatGPT o la que quieras. El prompt no tiene que ser largo: «Hacé una lista de supermercado sencilla y fácil de usar, con todo el código en un solo archivo».
2. **Mientras la IA trabaja, armá tu lista.** Abrí un bloc de notas y anotá qué cosas pensás que tiene que tener la app para ser sencilla y fácil de usar. Por ejemplo: ¿puedo agregar y borrar productos? ¿Puedo agregar apretando Enter? Cuando entro, ¿el foco ya está en el campo para escribir? ¿Me deja agregar un producto vacío? Vos decidís qué es importante para tu app. Todavía no abras el navegador ni la vista previa.
3. **Cuando termine, andá al código, no al navegador.** Buscá cada cosa de tu lista y anotá si está implementada y en qué parte del código. Si algo no lo entendés, primero intentá razonarlo vos. Si no sale, pedile una pista a la IA.
4. **Ahora sí, abrí la app en el navegador.** Compará lo que pasa con lo que anotaste leyendo el código. Si algo no coincide, volvé al código hasta entender por qué.
5. **Iterá hasta que quede simple.** Pedile a la IA que saque o cambie lo que sobra o está mal, y cada cambio leelo y probalo de nuevo. La idea es terminar con una app chica y fácil de usar, solo con lo que vos considerás básico.

Por ejemplo, pensemos en el foco al abrir la app. Seguramente tenga que ver con el input, así que vamos a buscarlo. En React, si el input tiene `autoFocus`, recibe el foco cuando se monta. Check:

```jsx
<label>
  Producto
  <input name="producto" autoFocus required />
</label>
```

Ojo, eso no significa que el foco vuelva al campo después de agregar un producto. Eso es otra cosa, y también la tenés que buscar en el código y probar.

**La meta:** mirar algo que hace la app y poder encontrar el código que lo hace.

### Ejercicio 2: Completions

Cuando hacemos una app desde cero, en realidad hacemos dos cosas: pensar qué tiene que hacer y descubrir cómo implementarla. Muchas veces creemos que lo tenemos claro, pero cuando empezamos a escribir aparecen dudas y cambios, nos mareamos y nos frustramos.

Pero ahora ya tenemos una app que funciona y sabemos lo que tiene que hacer. Nos podemos enfocar solo en implementarla.

1. **Creá un proyecto nuevo, desde cero,** y hacé la misma app otra vez, con la misma lista del ejercicio anterior.
2. **Escribila con completions,** o sea, las sugerencias que te aparecen en el editor mientras escribís (Copilot, Cursor o el que uses). Podés aceptarlas si entendés lo que hacen, pero no vale copiar y pegar código ni pedirle a un agente que te haga la app.
3. **Probala con tu lista.** Si te trabás mucho en alguna parte, anotala, seguí con otra cosa y volvé después. Si necesitás mirar cómo estaba hecho en el proyecto anterior, miralo como referencia, pero después escribilo vos.

**La meta:** pasar de entender el código a poder escribirlo, con una ayuda mientras escribís.

### Ejercicio 3: Escribirlo todo vos

Hacé la misma app por tercera vez, en un proyecto nuevo. Ahora apagá las completions y escribí vos el 100% del código. Podés leer documentación y usar las ayudas de sintaxis normales del editor.

A esta altura ya sabés qué tiene que hacer la app y ya la implementaste dos veces. Vas a tener casi todo el código en la cabeza, así que va a ser bastante mecánico: te acordás de las partes y te podés enfocar en escribirlas y en entender cómo se conectan.

Mientras la escribís, van a aparecer momentos de «ah, esta línea estaba por esto». O vas a pensar que algo sobra, lo vas a sacar, no va a andar y ahí vas a entender para qué servía. Ese es el momento en el que aprendés algo que te queda, y que posiblemente no hubieras aprendido solo leyendo el código.

Cuando termines, probala con tu lista y compará las tres versiones. Fijate qué cosas podés explicar ahora que antes no entendías.

**La meta:** escribir código no para escribirlo, sino para aprender, y así entender mejor el código que leés.

> ¿Querés otra vuelta? Hacé que cargar, agregar y borrar tarden un segundo. Pensá qué debería ver la persona mientras espera y qué pasa si hace otra cosa mientras tanto. Después hacé los tres ejercicios otra vez con ese cambio.

### Ejercicio 4: Llevar una solución a un cliente

Buscá algo chico para mejorar en un negocio o emprendimiento que tengas cerca y armá algo para mostrarle. Acá sí podés usar la IA para hacer el prototipo rápido, porque la meta es otra.

Buscá ideas que sean simples en tres sentidos: **poco código, poco tiempo de desarrollo y poco esfuerzo para que el cliente la empiece a usar**. Si la app te lleva dos horas pero el negocio tiene que cambiar toda su forma de trabajar, posiblemente no sea una buena primera propuesta.

1. **Encontrá algo concreto para resolver.** Por ejemplo, una carta por QR, un catálogo para armar pedidos o una agenda de actividades. Pensá también quién va a actualizar la información y cuánto trabajo le va a dar.
2. **Armá una demo chica.** Que resuelva una sola cosa y que la puedas mostrar en pocos minutos. Usá datos de ejemplo y no le agregues funcionalidades antes de saber si le interesan.
3. **Mostrala y escuchá.** Andá con algo que ya funcione, contale qué pensaste y preguntale si le serviría. Si le interesa, acuerden una prueba chica: qué incluye, qué tiene que aportar el negocio y cuánto va a costar, aunque esta primera vez sea gratis.

Podés arrancar la conversación así:

> Hola, estoy practicando desarrollo y armé esta demo pensando en tu negocio. Vi que [observación] y se me ocurrió [solución]. ¿Te la muestro y me decís si te sirve?

Hacé que probarla sea fácil: mandar un link o poner un QR es mucho menos trabajo que capacitar a todo el equipo o cargar cientos de productos. Si funciona, después hay tiempo para hacerla crecer.

**La meta:** resolverle algo útil a una persona real y aprender de lo que te diga. La demo abre la conversación, pero el cliente aparece cuando alguien acepta trabajar con vos.
