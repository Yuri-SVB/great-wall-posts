---
id: 009
título: "¿Esconder tu bitcoin todavía te protege?"
subtítulo: "Brasil tiene la peor estadística del mundo para el tipo de ataque en el que esconder no sirve, y el mercado sigue vendiendo escondites."
idioma: es
autor: Yuri da Silva Villas Boas
papers: [DS, DR]
tiempo_de_lectura: ~7 min
traducción_de: pt-BR.md
portada: assets/capa-1200x675.webp
portada_alt: "Un hombre levanta un cedazo para tapar el sol, y la luz atraviesa la malla. Es el equivalente brasileño de tapar el sol con un dedo."
---

# ¿Esconder tu bitcoin todavía te protege?

<p align="center"><img src="assets/capa-1200x675.webp" alt="Un hombre levanta un cedazo para tapar el sol, y la luz atraviesa la malla. Es el equivalente brasileño de tapar el sol con un dedo." width="680"></p>

**El consejo estándar para quien teme ser secuestrado por causa de su bitcoin
viene en tres partes: no se lo cuentes a nadie, niégalo si te preguntan, y ten un
*decoy* para entregar.**

**Las tres son apuestas sobre lo que el criminal va a *creer*. Y ninguna de ellas
ha sido nunca evaluada como lo que es: un mecanismo de seguridad cuya fuerza
entera depende de la ignorancia del adversario.**

Este texto sostiene que esconder bitcoin no solo es ineficaz. Es **autodestructivo a
escala**, y la cuenta cae sobre quien nunca siguió el consejo.

---

## Esconder bitcoin tiene nombre, número y antecedentes

Primero el vocabulario.

*Decoy*, o billetera señuelo. En Brasil lo llamamos "la plata del ladrón": un
monto menor, apartado a propósito para entregarlo en caso de robo.

En ingeniería de seguridad toda esa familia de tácticas está catalogada. Se llama
*Reliance on Security Through Obscurity*, registrada como
[CWE-656](https://cwe.mitre.org/data/definitions/656.html). En cualquier otro
dominio eso es un defecto de diseño. En custodia de bitcoin es el consenso.

### Esconder bitcoin es condescendiente por construcción

Este paradigma, que en diseño de protocolos se llama **oscuridad**, es
intrínsecamente condescendiente. Supone que el ladrón no es mentalmente capaz de
leer los mismos manuales, ver los mismos tutoriales y hacer los mismos cursos que
sus víctimas.

Si tú puedes aprender un procedimiento en internet, un ladrón también. Y por
supuesto sabrá que el procedimiento existe.

---

## Brasil está en el peor cuadrante del registro

Jameson Lopp mantiene desde hace años un [registro público de ataques físicos a
tenedores de bitcoin](https://github.com/jlopp/physical-bitcoin-attacks), los
llamados "$5 wrench attacks". Codifiqué los 351 incidentes del registro por
modalidad. El resultado por país no es uniforme: varía en un orden de magnitud.

| Jurisdicción | Incidentes | Secuestro | Robo a mano armada | Razón S:R |
|---|---:|---:|---:|---:|
| **Brasil** *(n pequeño)* | 12 | 75,0% | 8,3% | **9,0** |
| Francia | 61 | 57,4% | 8,2% | 7,0 |
| *Todos los incidentes* | 351 | 35,0% | 22,8% | 1,5 |
| Estados Unidos | 59 | 20,3% | 33,9% | 0,6 |
| Rusia *(n pequeño)* | 10 | 30,0% | 50,0% | 0,6 |

### Nueve secuestros por cada robo

Leé la columna de la derecha. En Estados Unidos el ataque típico es un robo: arma
apuntada, transferencia inmediata, minutos en escena.

En Brasil la proporción se invierte. **Por cada robo a mano armada registrado,
nueve secuestros.** El ataque brasileño no es un evento de minutos. Es un evento
de horas o días, con la víctima bajo control del criminal todo el tiempo.

### La salvedad viene junto, y es seria

El registro es una muestra de prensa, `n=12` para Brasil no sostiene nada por sí
solo, y la codificación es por palabra clave en titular, no por duración medida.
Trata la fila de Brasil como direccional.

La comparación que de verdad pesa es Francia contra Estados Unidos: dos
subconjuntos del mismo tamaño (61 y 59) con composiciones invertidas. La
composición sí varía con las condiciones locales, y las condiciones locales
brasileñas las conoce cualquiera que viva ahí.

Esto importa porque **toda la promesa de esconder bitcoin depende de que el ataque sea
corto**. Un decoy funciona si el criminal se lleva los ocho mil reales y se va. No
tiene respuesta para la pregunta siguiente, hecha al tercer día, en cautiverio.

---

## Qué pasa cuando todo el mundo está entrenado para negar

Acá está el mecanismo, y es económico antes que criptográfico.

### La credibilidad de una negativa es un recurso común

La produce el conjunto de todos los tenedores y la consume cada uno que niega.
Mientras negar es raro, negar carga información: el criminal actualiza su creencia
y tus chances de que te suelten suben.

Cuando negar se vuelve el guion esperado, cuando todo canal, todo curso y todo
grupo de Telegram enseñan la misma frase, **una negativa deja de cargar
información**.

El interrogatorio que empieza con "no tengo nada" no le da al criminal ninguna
actualización a tu favor. Y su continuación racional en ese punto no es soltarte.
Es insistir.

La respuesta individualmente racional a ese entorno es esconder mejor y ensayar
más. Lo que **agota el recurso todavía más, para todos**.

Lo llamé **Espiral de la Negación**, y su costo es una externalidad clásica: cae
sobre quien necesita ser creído. Incluso sobre quien usa un esquema que no depende
de mentir. Incluso sobre quien, honestamente, **no tiene bitcoin alguno**, y el
registro tiene casos así.

### El mercado vende el agotamiento como producto

Diversas consultorías, cursos y tutoriales de autocustodia listan, entre sus
servicios pagos, el armado de decoys con entrenamiento de credibilidad.

O sea: se paga para quedar fluido en una negativa que el criminal ya descuenta,
justamente por ser enseñada y vendida. El remedio degrada aquello que vende, y no
solo para el cliente.

---

## El problema más grave: no puedes probar que olvidaste

Hay una segunda falla, y es peor, porque es sobre el desenlace y no sobre la
duración.

Parte de un hecho simple e ineludible: **nadie puede probar que no sabe algo.**
Saber es demostrable; *no* saber, no. No tienes cómo probar que olvidaste la
contraseña, ni que no existe backup en ninguna parte.

### La Carrera Mortal

Ahora considera cualquier esquema que, después de tomar tu dispositivo, le deje al
criminal un camino **viable pero no concluido** hasta el dinero: un bloqueo
temporal, un rescate por delegado, una bóveda con retardo, una clave que todavía
hay que romper.

Te sueltan. Y no puedes probar que no guardaste una copia utilizable.

Lo que existe a partir de ahí es una **carrera** entre tú y él por el mismo
saldo. Y una carrera con un competidor al alcance de la mano crea algo que ningún
whitepaper de billetera menciona: **un incentivo material para eliminarte.** No por
crueldad. Por aritmética. Sacar al otro corredor de la pista es la jugada más
barata disponible.

Lo llamé **Carrera Mortal**. En el registro, al menos el 4,6% de los incidentes (16
de 351) traen víctima muerta, y ese número es un **piso**, no una estimación. Un
homicidio suele reportarse como homicidio, no como "ataque a tenedor de bitcoin".
El desenlace que el argumento predice está documentado en la práctica.

### Por qué el decoy es una máquina de zona gris

El criterio de diseño que sale de esto es seco: **un esquema de custodia resistente
a coerción solo puede admitir dos desenlaces. El ataque funciona claramente, o el
ataque fracasa claramente. Nunca una carrera.**

La zona gris es exactamente donde vive el incentivo al asesinato. Lo llamé
**Principio de Ausencia de Zona Gris**.

Fijate lo que eso le hace al decoy. Es, por construcción, una máquina de zona gris:
el criminal se va sospechando que hay más, y sin ninguna manera de cerrar la
sospecha. Es el peor lugar posible donde estar.

---

## Un caso brasileño que cierra el argumento

Porto Velho, octubre de 2019. Una banda secuestra a
[Arcilio Nogueira de Souza](https://archive.is/jyzcJ), ata a la víctima a un árbol
y la golpea durante horas. Los criminales **no se llevaron nada**. El celular no
daba acceso a los fondos.

Ese caso es el argumento entero en un párrafo. La inaccesibilidad de los fondos *no
terminó el ataque*. Lo **prolongó**.

El esquema "funcionó" en el sentido en que la industria mide, el dinero no salió, y
la persona pasó horas atada a un árbol recibiendo golpes, porque fuera de su cabeza
no había nada que cerrara la duda del criminal.

Por eso separo los dos mecanismos. La Carrera Mortal pone precio al **desenlace**.
La Espiral de la Negación pone precio a la **duración**. Un esquema puede ser
inocente de uno y culpable del otro, y la mayoría de lo que se vende hoy es
culpable de ambos.

---

## Qué queda, si esconder bitcoin no es defensa

Quedan tres rutas honestas, y conviene saber en cuál estás.

### 1. Física

Dispersión geográfica, bóvedas, multisig con custodia lejana. Funciona, y reduce la
seguridad del bitcoin a "qué tan buena es la bóveda". Bitcoin convertido en **oro
con pasos extra**, con un costo que escala con la defensa. Para la inmensa mayoría
es inaccesible.

### 2. Delegada

Alguien fuera del alcance del criminal guarda la pieza que falta: un exchange,
cocustodia, rescate por tercero. Limpia el criterio, pero cambia la premisa: la
custodia deja de ser individual. *Not your keys.* Y la ruta **se cierra** si el
delegado vive cerca tuyo.

### 3. Tácita

El secreto nunca estuvo en el dispositivo, y no es dictable ni bajo tortura, porque
es reconocimiento perceptual y no una frase. Incautar el aparato no entrega nada
viable. **Fracaso claro**, sin corredor sobrante, y la custodia sigue siendo
individual.

La tercera ruta es donde trabajo, y el proyecto se llama **Great Wall**. Acá va la
advertencia que cualquier texto honesto sobre esto necesita: **la implementación es
un prototipo. No pongas tus ahorros detrás todavía.**

Cuando eso cambie estará escrito, con fecha, en
[`DELIVERED.md`](https://github.com/Yuri-SVB/support/blob/main/DELIVERED.md), un
archivo versionado en git justamente para que "el trabajo avanza" sea una
afirmación auditable y no una promesa.

### El efecto colateral contraintuitivo

Hay un efecto colateral lindo en esta ruta: **un proyecto público y no oscuro
mejora la situación de quien niega.**

Un criminal que cree que hay un mecanismo eficaz en circulación está creyendo que
mentir no es la única herramienta disponible para la víctima, y una víctima con
alternativa real tiene menos motivo para mentir.

Esconder sigue siendo malo como defensa primaria. Pero no es indiferente qué
esquema acompaña.

---

## Qué vendo, y qué no vendo

**No vendo software.** Great Wall, BTC-D20, BIP-450 y los papers son MIT o
Apache-2.0, y eso no cambia: sin versión "pro", sin funcionalidad destrabada por
pago, sin fila preferencial para quien donó.

Está escrito en el [repositorio de apoyo](https://github.com/Yuri-SVB/support), y
está escrito ahí porque una promesa en un artículo no vale nada y una promesa en
git tiene fecha.

### Sí vendo consultoría de autocustodia

Es un servicio, y el servicio es este: miro el esquema que ya tienes, hardware
wallet, passphrase, multisig, señuelo, plan de herencia, lo que haya, y respondo
cuatro preguntas en un informe cerrado:

1. ¿Tu seguridad se apoya en algún **truco secreto**? ¿Depende de que el
   criminal no sepa qué haces, y cómo lo haces?
2. Una vez que el criminal tiene tus dispositivos y tus secretos, ¿podría gastar **en el
   acto**, o solo **al cabo de un tiempo**? "Al cabo de un tiempo" quiere decir
   que sigues siendo un corredor.
3. ¿Tu custodia es **estrictamente individual**? ¿Alguien más puede hacer algo
   que te impida llegar a tus propias monedas?
4. ¿Depende de **objetos concretos en lugares concretos**? ¿Y esos lugares son
   tuyos?

No es venta de producto: en la mayoría de las auditorías la recomendación es tocar
lo que ya existe, y en algunas el veredicto es que está razonable. Lo que no voy a
hacer es armar un decoy con entrenamiento de negativa, por el argumento entero de
arriba.

Contacto: **yuri@t3infosecurity.com**.

### Y si no quieres comprar nada

Los papers son gratuitos y no están detrás de ningún registro:
[*The Deadly Race*](https://zenodo.org/doi/10.5281/zenodo.22018891) (la carrera y el
criterio) y [*The Denial Spiral*](https://zenodo.org/doi/10.5281/zenodo.22778480) (la
espiral, la clasificación de los productos oscuros en el mercado y el método de
codificación del registro).

Los datos nuevos de incidentes van al
[registro de Lopp](https://github.com/jlopp/physical-bitcoin-attacks), y no a una
base de datos mía, porque esa información es patrimonio público y pertenece a
todos, incluido el próximo objetivo.

Si este texto te sirvió, [el apoyo va acá](https://github.com/Yuri-SVB/support).
Lightning y on-chain, sin contrapartida y sin registro.

---

*Yuri da Silva Villas Boas es criptógrafo aplicado, autor de la BIP-450 (Formosa) y
del protocolo Great Wall. Las dos afirmaciones centrales de este artículo están
desarrolladas formalmente en los papers citados, actualmente en evaluación
académica.*
