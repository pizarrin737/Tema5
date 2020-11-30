---

## Universidad de Costa Rica
### Escuela de Ingeniería Eléctrica
#### IE0405 - Modelos Probabilísticos de Señales y Sistemas

Segundo semestre del 2020

---

* Estudiante: **Jose Miguel Pizarro Viales**
* Carné: **B86079**
* Grupo: **1**

# `L5` - *Cadenas de Markov*

De los datos del problema se tiene: $\lambda = 2$. Para tener que el servidor no esté vacío (sin atender solicitudes) más del 10% del tiempo. Esta asignación se puede rescribir como que al menos halla 1 persona en el sistema el 90% del tiempo. De esta forma se tiene lo siguiente: 

$$
\begin{aligned}
P( \text{1 o más clientes en el sistema} ) = \rho & = \frac{\lambda}{\nu} \geq 0.9 \\
\nu & \leq \frac{\lambda}{0.9} = \frac{2}{0.9} = 2.222
\end{aligned}
$$

Por lo tanto, el servidor debe atender menos de 2.222 solicitudes por minuto para garantizar que el 90% del tiempo halla por lo menos una persona en el sistema. Por lo tanto, el codigo se adaptó para evaluar el sistema con este valor de $\nu$. De esta forma se obtuvieron los siguientes resultados:

<img align='center' src='https://github.com/pizarrin737/Tema5/blob/main/Resultado.png?raw=true' width='250'/>

De esta forma se puede observar que los resultados son satisfactorios, ya que precticamente siempre hay personas en el servidor.
