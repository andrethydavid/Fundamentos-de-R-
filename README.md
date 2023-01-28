Data Science y programación van de la mano, un programador debería conocer de ciencia de datos, pues estos se encargan de recolectar los datos a través de las interfaces y los datos son la materia prima para la data Science. Se hace un recuento de la revolución industrial (las revoluciones industriales). Hoy se vive la 4ª revolución industrial, IoT, AI, los datos se producen constantemente, las empresas nos conocen por los datos que producimos.

Big Data es muchísimo mayor a las 16 mil columnas. Volumen. Velocidad. Variedad son los requisitos, manejamos muchos datos no estructurados. Es decir, no en columnas. Se requieren conocimientos de matemáticas, estadística, programación, conocimiento de negocio y contexto, visualización y comunicación. Responder preguntas a través de los datos.

# Lenguaje De Programación De Datos R

Python y R son dos lenguajes potentes para manejar los datos. Para los que estamos empezando en el mundo de Ciencia de Datos es importante no centrarnos en la discusión de cual es mejor, sino entender que son dos lenguajes con los cuales podemos afrontar diversos proyectos y dependiendo del proyecto, sus características y alcance, deberíamos de elegir uno lenguaje u otro. Fundamental tener este concepto claro para empezar en este mundo.


Los primeros cálculos con R y variables.
Se puede seralizar sumas 

4 + 8  

restas 
5 - 8

multiplicacion 
7* 8

Variables abuscar 
oficina <-7
platzi < - 1 
transporte < - 1.5
tiempo_al_dia <- oficina + platzi + transporte
tiempo_al_dia

solucion de la variable 

> oficina <-7
> platzi < - 1 
[1] FALSE
> transporte < - 1.5
[1] FALSE
> tiempo_al_dia <- oficina + platzi + transporte
> tiempo_al_dia
[1] 9.5


variable de  notas 

corte_1 <- 0.3
corte_2 <- 0.3
corte_3 <- 0.4

nota_1 < - 4.0
nota_2 < - 4.6
nota_3 < - 3.0


nota_c_1 < - nota_1 * corte_1
nota_c_1


nota_c_2 < - nota_2 * corte_2
nota_c_2

nota_c_3 < - nota_3 * corte_3
nota_c_3

nota_final <- nota_c_1 + nota_c_2  +nota_c_3
nota_final 



COMANDO DE R 
str(NOMBRE DEL ARCHVO  QUE DESEAS VER LOS DATOS )
![image](https://user-images.githubusercontent.com/72534486/211956509-61a75c3d-357f-4b8f-b9f1-c983da125995.png)

es para ver si tienen nimero los integers ya que los integer son texto no numeros binarios 

el comando
? nombre de la carpeta es para ver la informacion 
![image](https://user-images.githubusercontent.com/72534486/211957193-7376f92f-c771-4da7-af5c-443eb3fc2746.png)

el siguiente comando es para que el int que no es int es un buliano es decir verdader y falso 
![image](https://user-images.githubusercontent.com/72534486/211958037-c6f818b2-33ca-4c1f-8391-6c094d88bbda.png)

summary(carpeta que uses ) es para desglosara la informacion o sumarla todo 
![image](https://user-images.githubusercontent.com/72534486/211958608-9ff21e62-93e7-46ac-bc3c-b5800f97f63a.png)

L variable para convertir  libras a kilos 
![image](https://user-images.githubusercontent.com/72534486/211960380-d3069eba-d451-4db1-9dc5-e8100a9072e3.png)
summary(mtcars)

wt <- (mtcars$wt*1000)/2
wt 

mtcars.new <- transform(mtcars,wt=wt*100/2)
mtcars.new


summary(mtcars.new)

Vectores 

tiempo_platzi <- c (25,5,10,15,10)
tiempo_lecturas <- c (30,10,5,10,15)
tiempo_aprendizaje <- tiempo_platzi +tiempo_lecturas
tiempo_aprendizaje
respuesta 
[1] 55 15 15 25 25

dias_aprendizaje <- c ("lunes","Martes","mircoles","jueves","viernes" )
dias_aprendizaje
[1] "lunes"    "Martes"   "mircoles" "jueves"   "viernes" 

Total_tiempo_platzi <- sum (tiempo_platzi)
Total_tiempo_platzi
total_tiempo_lecturas <- sum(tiempo_lecturas)
total_tiempo_lecturas
total_tiempo_adicional <- Total_tiempo_platzi + total_tiempo_lecturas
total_tiempo_adicional
![image](https://user-images.githubusercontent.com/72534486/212226602-10862d1c-7e81-4319-b863-e9329a8fc840.png)

bulianos

dias_mas_20min <- c(TRUE,FALSE,FALSE,TRUE,TRUE)
dias_mas_20min
![image](https://user-images.githubusercontent.com/72534486/212226840-e0929df6-b537-45e5-ac71-51f530a66267.png)

Matrices

![image](https://user-images.githubusercontent.com/72534486/212231124-6f80fcd8-d2b6-40de-aa8a-5c676b252ba7.png)
![image](https://user-images.githubusercontent.com/72534486/212231158-7d791cac-93d9-4974-9a96-6f6171c04262.png)
Code
#matriz

#CREO MATRICES . NTW = NUMERI DE FILAS;BYNOW = PARA QUE SE ORDNE POR FILAS 

tiempo_matrix <- matrix(c(tiempo_platzi, tiempo_lecturas),
                        nrow=2, byrow=TRUE)

#CREAR ETIQUETAS DE MATRICES Y CREO VARIABLES PARA GUARDARLAS:

dias <- c("Lunes", "Martes", "Miercoles", "Jueves", "Viernes")
Tiempo <- c("tiempo_platzi", "tiempo_lecturas")

#asignamos cual era la fila y cual la columna 

colnames(tiempo_matrix) <- dias
rownames(tiempo_matrix) <- Tiempo

tiempo_matrix
#llamo la matriz
colSums(tiempo_matrix)
rowSums(tiempo_matrix)


.
