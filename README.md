# Estudios Sobre Markdown

```
Representaremos aquellos comandos para poder 
representar los beneficios de trabajar con Markdown
```
## Título, \# usandolo
## Sub título, \## usandolo
### sub título, \### usandolo

```
la \# se usa para comentar los comandos de Markdown
```

**Negrita**,    Usandolo los *** se coloca en negrita

_Italica_ ,    \# _ se coloca en Italica

***Si quisiera tener una letra negrita y curveada***. \# Seria con ***

***Una cita, se optiene con*** \> y **
>A la vista de suficientes ojos, una falla resulta evidente **Linux Torval


```
Esta sección escribiremos un poco de código esperando que sea de su agrado para ver la prueba de las birgulillad
```
**Una lista desordenada*
 +  Primera opción
 +  Segunda opción 
    *   Caso a
    *   Caso b
 +  Tercera opción

**Una lista ordenada*
 1. Primera opción
 2. Segunda opción 
    1. Caso a
    2. Caso b
 3. Tercera opción


**Trabajaremos con Link**

Visita mi **[Perfil](www.google.com "Google")**

**Para referenciar mi correo electrónico :**
<r_trelles@hotmail.com>

**Referencias:**
Esto es una referencia [1]

[1]: https://www.google.com

**Para Cargar imagenes**
```
Se coloca el signo de !
![Esta es la imagen de internet](Ruta)
```
![Imagen a Mostrar](https://concepto.de/wp-content/uploads/2018/02/sistemas-de-informacion-768x399.jpg  "Hola, Bienvenidos")


**Insertando Insignias**

![Hola](https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=Tableau&logoColor=white) 
![](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)

```

Una Páguina que tiene una base de Insignias
https://github.com/alexandresanlim/Badges4-README.md-Profile

https://shields.io/

```
[Link de Insignias](https://github.com/alexandresanlim/Badges4-README.md-Profile)

![veamos](https://github-readme-streak-stats.herokuapp.com/?user={RaulTrelles})

![Link de Insignias fijas](https://shields.io/)

**6.- Reglas y Emojis, Haciendo una linea trasversal grusa**
***
salva a los panda :panda_face: :sleeping:

Link de Emoticones: [Link de emiticones](https://www.webfx.com/tools/emoji-cheat-sheet/) :grin:

**7.- Tablas**
|Cabecera 1 | Cabecera 2 | Cabecera 3|
|-----------|------------|-----------|
|asasasasssa|asasasasasas|sasasasasas|
|           |            |           |

**8.- Combinacion de MD y HTML**
Se ppueden usar etiquetas de html

**9.- Visualizacion de veideos**
[![veamos el siguiente video]](https://www.youtube.com/watch?v=1BzzckYqT9w&list=PLM4HZoZrNapsQ_f6a9275n15riyr-2AnQ&index=9 imagenalternativa.jpg](https://www.youtube.com/watch?v=1BzzckYqT9w&list=PLM4HZoZrNapsQ_f6a9275n15riyr-2AnQ&index=9)

**10.-Funciones para textos**

<ins>Texto subrrallado</ins>

<center>Texto al centro</center>

<p style="color:red"> Texto de color </p>
<p style="color:green"> Texto de color </p>

**<ins>10.1.- links</ins>**

_misma ventana_

[TESTO PARA EL lINK](https://www.google.com)

_otra ventana_

<a href="https://www.google.com" target="_blank"> TEXTO PARA LINK EN OTRA PAGUINA </a>


**11.- Manejar diagramas de flujo**


```mermaid
graph
A[Square React] -- link text --> B((circle))
A --> C(Round React)
B --> D(Rhombus)
```
##

```mermaid
graph LR
A[Square React] -- link text --> B((circle))
A --> C(Round React)
B --> D(Rhombus)
```
##
```mermaid
flowchart TB
A((Inicio))
B[/Escribe la contraseña/]
C[\PASS\]
D{pass =1234}
E[/ Felicidades login correcto /]
F[/ Loggin correcto /]
G((Fin))

A --> B --> C --> D

D --> | VERDADERO| E

D --> |FALSO| F

F --> B

E --> G
```
##
```mermaid
  graph TD
      A-->B;
      A-->C;
      B-->D;
      C-->D;
```
##
```mermaid
flowchart LR;
    A-->B;
    B-->C;
    C-->D;
    click A callback "Tooltip for a callback"
    click B "http://www.github.com" "This is a tooltip for a link"
    click A call callback() "Tooltip for a callback"
    click B href "http://www.github.com" "This is a tooltip for a link"
```
**12.- Diagrama de secuencia**

```mermaid
sequenceDiagram
    participant Alice
    participant John
    links Alice: {"Dashboard": "https://dashboard.contoso.com/alice", "Wiki": "https://wiki.contoso.com/alice"}
    links John: {"Dashboard": "https://dashboard.contoso.com/john", "Wiki": "https://wiki.contoso.com/john"}
    Alice->>John: Hello John, how are you?
    John-->>Alice: Great!
    Alice-)John: See you later!
```
##
```mermaid
  flowchart LR;
      A[CI MULTI CHAPTCHA]-->B{Select captcha service by developer?};
      classDef green color:#022e1f,fill:#00f500;
      classDef red color:#022e1f,fill:#f11111;
      classDef white color:#022e1f,fill:#fff;
      classDef black color:#fff,fill:#000;
      B--YES-->C[How to use?]:::green;
      
      C-->U[I choose recaptcha.]:::green;
      U--Views-->Q["echo CIMC_JS('recaptcha');\n echo CIMC_HTML(['captcha_name'=>'recaptcha']);"]:::green;
      U--Controller-->W["CIMC_RULE('recaptcha');"]:::green;
      
      C-->I[I choose arcaptcha.]:::white;
      I--Views-->O["echo CIMC_JS('arcaptcha');\n echo CIMC_HTML(['captcha_name'=>'arcaptcha']);"]:::white;
      I--Controller-->P["CIMC_RULE('arcaptcha');"]:::white;
      
      C-->X[I choose bibot.]:::red;
      X--Views-->V["echo CIMC_JS('bibot');\n echo CIMC_HTML(['captcha_name'=>'bibot']);"]:::red;
      X--Controller-->N["CIMC_RULE('bibot');"]:::red;
      
      B--NO-->D[How to use?]:::black;
      D---Views:::black-->F["echo CIMC_JS('randomcaptcha');\n echo CIMC_HTML(['captcha_name'=>'randomcaptcha']);"]:::black; 
      D---Controller:::black-->T["CIMC_RULE('archaptcha,recaptcha,bibot');"]:::black;
```
##
```mermaid
sequenceDiagram
    participant dotcom
    participant iframe
    participant viewscreen
    dotcom->>iframe: loads html w/ iframe url
    iframe->>viewscreen: request template
    viewscreen->>iframe: html & javascript
    iframe->>dotcom: iframe ready
    dotcom->>iframe: set mermaid data on iframe
    iframe->>iframe: render mermaid
```
**13.- Graficas circulares**

```mermaid
pie showData
    title Lenguajes más Usados en el proyecto
            "React":50
            "html":20
            "c++":20
            "vfox":10

```

*14.- Diagramas entidad relación*
```mermaid
erDiagram

producto {
    string id_producto
    string nombre
    double precio
}
usuarios {
     string id_user
     string nombre
     string direccion       
}
pedido {
    string id_pedido
    string id_user
    string id_producto
}

usuarios ||--o{ pedido : compra
producto }|--o{ pedido : venta

```
*15.- Como crear diagramas journey*

```mermaid
journey 
    title Compra
    section seleccion de productos
        Navegar: 6  :usuario
        Agregar al carrito: 6: usuario
    section Pago
        Realizar Pago:  3: usuario
        Validar Pago:   5: sistema       

```
##

*6.- Como crear un diagrama git*
```mermaid
gitGraph
    commit
    branch dev
    commit
    commit
    checkout main
    commit
    merge dev
    commit id: "v.1.0.0" tag:   "release"
    checkout dev
    commit
    branch bug
    commit id:  "error 484"
    checkout dev
    commit
    checkout bug
    merge dev
    checkout main
    commit
    commit
    merge dev
    commit id:  "v.2.0.0" tag:  "Release"

```
====

*17.- Diagramas de Gantt*
```mermaid
gantt
    dateformat  YYYY-MM-DD
    excludes weekends
    title   proyect tienda online

    section Diseño
        Diseño BD.  :   crit,   DB, 2022-07-20,   7d
        Diseño Frontend : F, 2022-07-20,    7d

    section Desarrollo
        Conexion DB :   active,   CDB,    after   DB, id
        Desarrollo Front    :   DF, after F, 4d

```
===

*17.- Diagramas de Gantt*
```mermaid
requirementDiagram

performanceRequirement TiempoDeCarga{
    id : 1
    Text : "Tiempo de carga menor a 2 seg"
    Risk : Low
    veriFymethod: Test
}

element Carga{
    type: user_experience
    docRef : gitHub/Test
}

Carga = satisfies --> TiempoDeCarga

```
# Personalizando perfil

crear un repositorio con nuestro nombre y editar el repositorio.
