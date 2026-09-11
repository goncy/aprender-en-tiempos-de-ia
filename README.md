# Aprender en tiempos de IA

Cuatro ejercicios para leer más código, aprender escribiéndolo y encontrar oportunidades con clientes reales. Hacelos con la tecnología que ya estés usando y a tu ritmo.

[Slides de la charla](https://www.figma.com/slides/u9hMhTKBKHKe04UqdW20xq) · [Video con los ejercicios](https://www.youtube.com/watch?v=UoRvcQ9avgw)

### Ejercicio 1: Versión solo IA

Vamos a usar una app generada por IA para practicar cómo leer código y entender qué hace.

1. **Pedile a una IA una app sencilla**, como una lista de tareas o de supermercado. Un pedido breve alcanza: «Hacé una lista de supermercado sencilla y fácil de usar, con la implementación en un solo archivo».
2. **Sin abrir el navegador ni la vista previa**, y mientras la IA trabaja, escribí tu lista de esperables: las cosas que considerás esenciales para esa app. Por ejemplo, agregar y borrar productos, enviar con Enter, tener el foco en el campo al abrir y rechazar productos vacíos. Elegí lo que te importa a vos.
3. **Buscá cada esperable en el código.** Anotá si creés que está implementado y qué código lo demuestra. Si no entendés algo, intentá razonarlo primero; después podés pedirle una pista a la IA.
4. **Ahora sí, probá la app en el navegador.** Compará lo que pasa con lo que habías deducido leyendo. Si no coincide, volvé al código hasta entender por qué.
5. **Corregí y repetí.** Podés pedirle cambios a la IA, pero volvé a leerlos y probarlos. Sacá lo que consideres innecesario hasta quedarte con una app pequeña y fácil de usar.

Por ejemplo, en React este campo recibe foco al montarse:

```jsx
<label>
  Producto
  <input name="producto" autoFocus required />
</label>
```

Pero eso no demuestra que el foco vuelva al campo después de agregar un producto. Esa es otra conducta que tenés que buscar y probar.

**La meta:** poder relacionar lo que hace la app con el código que lo implementa.

### Ejercicio 2: Completions

Cuando programamos, muchas veces se mezclan dos problemas: decidir qué queremos hacer y descubrir cómo implementarlo. Esa falta de claridad nos hace cambiar de rumbo, confundirnos y frustrarnos.

Ahora ya tenemos una app que funciona y sabemos qué debe hacer. Podemos concentrarnos en implementarla.

1. **Creá un proyecto nuevo** y reconstruí la misma app, con los mismos esperables del ejercicio anterior.
2. **Escribí usando completions:** las sugerencias de IA que aparecen mientras tipeás en el editor. Podés aceptarlas si entendés qué hacen, pero no copiar y pegar implementaciones ni pedirle a un agente que escriba la app completa.
3. **Probá con la misma lista de esperables.** Si algo te bloquea mucho, dejalo anotado y seguí con otra parte; volvé después. Si necesitás mirar una implementación anterior, usala como referencia y luego escribila vos.

**La meta:** pasar de reconocer una implementación a poder construirla, con ayuda mientras escribís.

### Ejercicio 3: Escribirlo enteramente

Rehacé la misma app una tercera vez, desde cero. Esta vez, desactivá las completions de IA y escribí vos todo el código de la aplicación. Podés consultar documentación y usar las ayudas habituales de sintaxis del editor.

A esta altura ya decidiste qué hacer y recorriste su implementación dos veces. El trabajo empieza a ser más mecánico: recordás las partes y podés dedicar tu atención a escribirlas y entender cómo se conectan.

Mientras escribís, van a aparecer esos momentos de «ah, por esto estaba esta línea» o «pensé que podía sacarlo, pero ahora entiendo para qué servía». Escribir, equivocarte y corregir te ayuda a aprender cosas que podías pasar por alto al leer.

Al terminar, probá los mismos esperables y compará las tres versiones. Fijate qué podés explicar ahora que antes no entendías.

**La meta:** escribir código como una forma de aprender y, con esa experiencia, también aprender a leerlo mejor.

> ¿Querés otra vuelta? Agregá un segundo de espera al cargar, agregar y borrar elementos. Pensá qué debería ver la persona mientras espera y qué pasa si hace otra acción. Después repetí los tres ejercicios con esa pequeña complejidad.

### Ejercicio 4: Llevar una solución a un cliente

Buscá una mejora pequeña para un negocio o emprendimiento cercano y prepará algo que puedas mostrarle. En este ejercicio podés usar IA para avanzar rápido con el prototipo.

Elegí ideas que sean simples en tres sentidos: **poco código, poco tiempo de desarrollo y poco esfuerzo para que el cliente las empiece a usar**. Una app que tarda dos horas en construirse pero obliga al negocio a cambiar toda su forma de trabajar puede ser una mala primera propuesta.

1. **Encontrá una oportunidad concreta.** Por ejemplo, una carta accesible por QR, un catálogo para armar pedidos o una agenda pública de actividades. Preguntate también quién actualizaría la información y cuánto trabajo le daría.
2. **Prepará una demo pequeña.** Resolvé un solo recorrido que puedas mostrar en pocos minutos. Usá datos de ejemplo y evitá sumar funciones antes de saber si interesan.
3. **Mostrala y escuchá.** Acercate con algo funcionando, explicá qué pensaste y preguntá si le serviría. Si hay interés, acuerden una prueba pequeña: qué incluye, qué necesita aportar el negocio y qué va a costar, aunque esa primera entrega sea gratuita.

Podés empezar la conversación así:

> Hola, estoy practicando desarrollo y armé esta demo pensando en tu negocio. Vi que [observación] y se me ocurrió [solución]. ¿Te la puedo mostrar y me contás si te serviría?

Buscá que probarla sea fácil: compartir un enlace o poner un QR suele requerir menos esfuerzo que capacitar a todo el equipo o cargar cientos de productos. Si la propuesta sirve, van a tener oportunidades de ampliarla después.

**La meta:** resolver algo útil para una persona real y aprender de su devolución. Una demo lista abre la conversación; el cliente aparece cuando alguien acepta trabajar con vos.
