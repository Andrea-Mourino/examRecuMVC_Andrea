# Explicacion Examen
1. Cree las clases ```Model```, ```Controller```, ```App``` y ```Calculadora```
2. Modifiqué el ```Main``` y lo llamé ```View``` (por comodidad y gusto personal) y llame en la ```App``` al *View.menu* 
3. Para empezar a programar comencé por lo primero, que seria ```Calculadora``` y cree 4 *int* llamados ```suma```, ```resta```, ```division``` y ```multiplicacion``` y luego dos *double* llamados ```numero1``` y ```numero2```
4. En el ```Model``` cree 4 *public static double* (porque si es int, no pilla los valores de ```numero1``` y ```numero2```) y metí la formula de la suma, resta, division y multiplicacion para que funcionara

```
  public static double sumarNumerosM(double numero1, double numero2) {
    return numero1 + numero2;
  }
  public static double restarNumerosM(double numero1, double numero2) {
    return numero1 - numero2;
  }

  public static double multiplicarNumerosM(double numero1, double numero2) {
    return numero1 * numero2;
  }

  public static double dividirNumerosM(double numero1, double numero2) {
    return numero1 / numero2;
  }
```
(Los llamé a todos con una M al final de Model. Es por gusto propio para que los diference mejor y no me confunda)

5. Ahora pasamos al ```Controller``` y lo que hice fue hacer otro *public static double* y agarrar los valores *double* ```numero1``` y ```numero2```. Luego llamamos al ```Model``` y le metemos los mismo valores que le agregamos antes, ya que es muy importante hacerlo en el mismo orden porque si no dará error

```
  public static double sumaC(double numero1, double numero2) {
    return Model.sumarNumerosM(numero1, numero2);
  }

  public static double restarC(double numero1, double numero2) {
    return Model.restarNumerosM(numero1, numero2);
  }

  public static double multiplicacionC(double numero1, double numero2) {
    return Model.multiplicarNumerosM(numero1, numero2);
  }

  public static double divisionC(double numero1, double numero2) {
    return Model.dividirNumerosM(numero1, numero2);
  }
```
(Hice lo mismo que en el Model y lo llame con una C al final de Controller)

6. Para terminar vemos que todo funcione correctamente (sin olvidar de hacer commits durante el proceso claramente) y ya estaría



# Examen recuperación MVC
---
Transforma esta aplicación según la arquitectura MVC vista en clase, sin cambiar la funcionalidad

Valoración:

* Clases por separado
* Funcionalidad de la vista (20 puntos)
* Funcionalidad del Controller (20 puntos)
* Utilización de Clase para guardar datos (como la clase Coche utilizada en clase) (20 puntos)
  * Coherencia con la clase Model (10 puntos)
* Realización de commits por cada paso que se realice (10 puntos)
* Comentarios en el código (5 puntos)
* Readme justificando la toma de desición y describiendo los beneficios aportados por el cambio de código (15 puntos)