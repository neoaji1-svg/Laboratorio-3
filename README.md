
# Laboratorio #3  👾​🗂️​🪟​

🗓️​ Fecha: 13/09/26

## Contenido ​📂​
En este laboratirio llevamos acabo la realizacion de tres programas el primero trata de un caso de estudio de DataGridView, el segundo programa trata de un caso de un juego, en esta ocasion se denomino como caso de juego Craps, y por ultimo se trato de la relizacion de un MDI(vetana padre y ventrana hija)

## Tecnologias usadas ​👨🏻‍💻​
* **Lenguaje / Framework:** C# (.NET / Windows Forms / .NET Core Console)
* **IDE / Herramientas:** Visual Studio / Visual Studio Code, Git, GitHub

## Capturas de pantalla ​🖥️​

**Caso de estudio de DataGridView** 🗂️​​
![image alt](https://github.com/neoaji1-svg/Laboratorio-3/blob/86f9008feefd256960f1854e12ec377520e79562/Programa%201.png)

Se diseñó un formulario de registro respaldado por una clase modelo Persona con propiedades autoimplementadas (Id, Nombres, Apellidos, Correo, FechaNacimiento, Salario). Los registros se gestionan dinámicamente utilizando una colección de tipo ArrayList enlazada directamente como fuente de datos (DataSource) del control DataGridView. Para garantizar la integridad de la entrada de datos, se incorporó el control DateTimePicker para selección visual de fechas y un componente ErrorProvider para validación en tiempo real. Además, se implementaron métodos estáticos auxiliares en una clase Utilidades para la verificación de campos vacíos y la validación de formato de correo electrónico mediante expresiones regulares (Regex).

<hr>
**Caso de juego Craps** 👾​
![image alt](https://github.com/neoaji1-svg/Laboratorio-3/blob/86f9008feefd256960f1854e12ec377520e79562/Programa%202.png)

Se implementó la lógica completa del juego de dados Craps orientado a objetos utilizando la clase Random de C# para la generación de lanzamientos aleatorios entre 1 y 6. Se definieron enumeraciones (enum) para representar los estados del juego (GANO, PERDIO, CONTINUA) y las reglas para combinaciones especiales de tiro (DOS_UNOS, TRES, SIETE, ONCE, DOCE). La lógica evalúa la primera tirada mediante una estructura switch con conversión explícita (casting) del tipo entero a enumeración. Si la suma inicial establece un Punto, el programa entra en un ciclo controlado para continuar tirando hasta repetir el punto (ganar) o sacar un 7 (perder).

<hr>

**MDI** 🪟​
![image alt](https://github.com/neoaji1-svg/Laboratorio-3/blob/86f9008feefd256960f1854e12ec377520e79562/Programa%203.png)

Se construyó un contenedor MDI (Multiple Document Interface) configurando la propiedad IsMdiContainer = true en el formulario principal padre. Para la navegación y control de la interfaz, se acopló un componente ToolStrip en la parte superior. La apertura de formularios hijos se programó asignando la propiedad MdiParent = this antes de invocar el método .Show(). Adicionalmente, para evitar instancias duplicadas y sobreposición de ventanas, se utilizó consulta LINQ sobre Application.OpenForms junto al método .BringToFront(), permitiendo reenfocar un formulario en pantalla si ya se encontraba previamente abierto

## Autor
+ Nombre: Neo Aji
+ Institución: Universidad Tecnológica de Panamá (UTP)
+ Fecha de Realización: [13/09/26]
