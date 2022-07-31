# Libreria de colores para C / C++ 🎨

Permite modificar el **color de fuente**  del texto y **color de fondo** en consola al momento de ejecucion.

<img style="display: inline" src="https://i.ibb.co/CKNJHLr/Screenshot-2.jpg" alt="Screenshot-2" border="0">

<img style="display: inline" src="https://i.ibb.co/ygMhPwX/fondos.jpg" alt="fondos" border="0">

*( font color and background color )*

---

## Comenzando 🚀

_Estas instrucciones te permitirán obtener una copia del proyecto en funcionamiento en tu máquina local para propósitos de desarrollo y pruebas._



### Pre-requisitos 📋

_Dependiendo del lenguaje que se utilice se necesita una libreria u otra_

* En **C**
```c
#include <stdio.h>
```
* En **C++**
```cpp
#include <iostream>
```

### Instalación 🔧

1. Descargar el zip o el archivo libreria "colors.h" 
2. Incluir el archivo ***colors.h*** en el directorio de tu programa / proyecto
3. Importarla desde tu archivo **C** ó **C++** con:      

         
```cpp
#include "colors.h"
```

## Despliegue 📦

_La libreria se basa en codigos de colores a traves de ANSI Escape codes_

<table style="width:70%">
  <thead>
    <tr>
    <th align="center\">Color</th>
    <th align="center">Font code</th>
    <th align="center">Background code</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><span style="color: black; --darkreader-inline-color:#e8e6e3;" data-darkreader-inline-color="">Black</span></td>
      <td align="center"><code>\x1B[30m</code></td><td align="center"><code>\x1B[40m</code></td>
    </tr>
    <tr>
      <td align="center"><span style="color: red; --darkreader-inline-color:#ff1a1a;" data-darkreader-inline-color="">Red</span></td>
      <td align="center"><code>\x1B[31m</code></td>
      <td align="center"><code>\x1B[41m</code></td>
    </tr>
    <tr>
      <td align="center"><span style="color: green; --darkreader-inline-color:#72ff72;" data-darkreader-inline-color="">Green</span></td>
      <td align="center"><code>\x1B[32m</code></td>
      <td align="center"><code>\x1B[42m</code></td>
    </tr>
    <tr>
      <td align="center"><span style="color: yellow; --darkreader-inline-color:#ffff1a;" data-darkreader-inline-color="">Yellow</span></td>
      <td align="center"><code>\x1B[33m</code></td>
      <td align="center"><code>\x1B[43m</code></td>
    </tr>
    <tr>
      <td align="center"><span style="color: blue; --darkreader-inline-color:#337dff;" data-darkreader-inline-color="">Blue</span></td>
      <td align="center"><code>\x1B[34m</code></td>
      <td align="center"><code>\x1B[44m</code></td>
    </tr>
    <tr>
      <td align="center"><span style="color: magenta; --darkreader-inline-color:#ff1aff;" data-darkreader-inline-color="">Magenta</span></td>
      <td align="center"><code>\x1B[35m</code></td>
      <td align="center"><code>\x1B[45m</code></td>
    </tr>
    <tr>
      <td align="center"><span style="color: cyan; --darkreader-inline-color:#1affff;" data-darkreader-inline-color="">Cyan</span></td>
      <td align="center"><code>\x1B[36m</code></td>
      <td align="center"><code>\x1B[46m</code></td>
    </tr>
    <tr>
      <td align="center"><span style="color: white; --darkreader-inline-color:#e8e6e3;" data-darkreader-inline-color="">White</span></td>
      <td align="center"><code>\x1B[37m</code></td>
      <td align="center"><code>\x1B[47m</code></td>
    </tr>
    <tr>
      <td align="center">Cualquier color (con V en [0-255])</td>
      <td align="center"><code>\x1B[38;5;Vm</code></td>
      <td align="center"><code>\x1B[48;5;Vm</code></td>
    </tr>
    <tr>
      <td align="center">Cualquier RGB color (Con valores en [0-255])</td>
      <td align="center"><code>\x1B[38;2;R;G;Bm</code></td>
      <td align="center"><code>\x1B[48;2;R;G;Bm</code></td>
    </tr>
    </tr>
  </tbody>
</table>


_Siendo **38** el numero para colores personalizados_

----


<table style="width:70%">
  <caption style=""><i>Colores disponibles</i></caption>

  <tr>
    <th>Name</th>
    <th  style="text-align:right">Code</th>
    <th></th>
  </tr>
  <tr>
    <th>Color</th>
    <th>Font </th> 
    <th>Background </th>
  </tr>
  <tr>
    <td>Rojo</td>
    <td style="color:RED">RED</td>
    <td style="background-color:red">BG_RED</td>
  </tr>
  <tr>
    <td>Verde claro</td>
    <td style="color:rgb(17, 245, 120)">LGREEN</td>
    <td style="background-color:rgb(17, 245, 120) ;color:black">BG_LGREEN</td>
  </tr>
  <tr>
    <td>Verde </td>
    <td style="color:green">GREEN</td>
    <td style="background-color:GREEN">BG_GREEN</td>
  </tr>
  <tr>
    <td>Amarillo</td>
    <td style="color:YELLOW">YELLOW</td>
    <td style="background-color:YELLOW;color:black">BG_YELLOW</td>
  </tr>
  <tr>
    <td>Cyan</td>
    <td style="color:CYAN">CYAN</td>
    <td style="background-color:CYAN;color:black">BG_CYAN</td>
  </tr>
  <tr>
    <td>Azul claro</td>
    <td style="color:rgb(53,149,240)">LBLUE</td>
    <td style="background-color:rgb(53,149,240)">BG_LBLUE</td>
  </tr>
  <tr>
    <td>Azul</td>
    <td style="color:BLUE">BLUE</td>
    <td style="background-color:BLUE">BG_BLUE</td>
  </tr>
  <tr>
    <td>Pink</td>
    <td style="color:#ff80c0">ROSE</td>
    <td style="background-color: #ff80c0 ">BG_ROSE</td>
  </tr>
  <tr>
    <td>Magenta</td>
    <td style="color:MAGENTA">MAGENTA</td>
    <td style="background-color:MAGENTA">BG_MAGENTA</td>
  </tr>
  <tr>
    <td>Blanco</td>
    <td style="color:WHITE">WHITE</td>
    <td style="background-color:WHITE;color:black">BG_WHITE</td>
  </tr>
  <tr>
    <td>Naranja</td>
    <td style="color:ORANGE">ORANGE</td>
    <td style="background-color:ORANGE;color:black">BG_ORANGE</td>
  </tr>
  <tr>
    <td>Gris</td>
    <td style="color:rgb(176, 174, 174)">GRAY</td>
    <td style="background-color:rgb(176, 174, 174);color:black">BG_GRAY</td>
  </tr>
  <tr>
    <td>Negro</td>
    <td style="color:Black">BLACK</td>
    <td style="background-color:Black;color:white">BG_BLACK</td>
  </tr>
</table>

-----

## Wiki 📖

Para cambiar el color de la fuente se es necesario concatenar el **Font code** de su respectivo color, con el mensaje a mostrar.

* En **C**
```c
#include <stdio.h>
#include "colors.h"

int main () {
 
  printf( RED      " This text is RED!     \n" );
  printf( LGREEN   " This text is LGREEN!  \n" );
  printf( GREEN    " This text is GREEN!   \n" );
  printf( YELLOW   " This text is YELLOW!  \n" );
  printf( BLUE     " This text is BLUE!    \n" );
  printf( ORANGE   " This text is ORANGE   \n" );
  printf( MAGENTA  " This text is MAGENTA! \n" );
 
  return 0;
}
```

* En **C++**
```cpp
#include <iostream>
#include "colors.h"

using namespace std;

int main () {
 
  cout << RED     << " This text is RED!     " << endl;
  cout << LGREEN  << " This text is LGREEN!  " << endl;
  cout << GREEN   << " This text is GREEN!   " << endl;
  cout << YELLOW  << " This text is YELLOW!  " << endl;
  cout << BLUE    << " This text is BLUE!    " << endl;
  cout << ORANGE  << " This text is ORANGE   " << endl;
  cout << MAGENTA << " This text is MAGENTA! " << endl;
 
  return 0;
}
```

*Salida:*


> <a href=""><img src="https://i.ibb.co/CKNJHLr/Screenshot-2.jpg" alt="Screenshot-2" border="0"></a>
---
Para cambiar el color de fondo se necesita la clave **RESET** al final de la instruccion.

1. Se concatena al inicio el Background_color a utilizar 
2. Se finaliza el mensaje con el codigo RESET
  
```cpp
#include <iostream>
#include "colors.h"

using namespace std;

int main () {
  cout << RED     <<BG_YELLOW << "This text is RED!      " << RESET << endl;
  cout << LGREEN  <<BG_CYAN   << "This text is LGREEN!   " << RESET << endl;
  cout << GREEN   <<BG_RED    << "This text is GREEN!    " << RESET << endl;
  cout << YELLOW  <<BG_GREEN  << "This text is YELLOW!   " << RESET << endl;
  cout << CYAN    <<BG_MAGENTA<< "This text is CYAN!     " << RESET << endl;
  cout << BLUE    <<BG_LGREEN << "This text is BLUE!     " << RESET << endl;
  cout << ORANGE  <<BG_BLUE   << "This text is ORANGE!   " << RESET << endl;
  cout << MAGENTA <<BG_ORANGE << "This text is MAGENTA!  " << RESET << endl;
 
  return 0;
}
```

*Salida:*

> <a href=""><img src="https://i.ibb.co/ygMhPwX/fondos.jpg" alt="fondos" border="0"></a>

### ⚠ ❗ **Precaucion** ❗ ⚠
No tomar en cuenta la sentencia **RESET** puede provocar que el background_color se corra a la siguiente linea o al fin de la consola.

## Autores ✒️

_Aquellos que ayudaron a levantar el proyecto desde sus inicios_

* **Jesús Alfonzo** - *Programación* - [Alfonzzoj](https://github.com/Alfonzzoj)

## Colabora 💭

Estan abiertas las colaboraciones para mas colores personalizados.

## Expresiones de Gratitud 🎁
* Comenta a otros sobre este proyecto 📢.
* No olvides dejarme una ⭐.
* Da las gracias públicamente 🤓.


