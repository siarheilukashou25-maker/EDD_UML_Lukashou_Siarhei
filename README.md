# EDD_UML_Lukashou_Siarhei

**Fase 1: Investigación Técnica**
-------
**Fork** - es un nodo de bifurcación con un punto de entrada y múltiples puntos de salida, que se utiliza para dividir el flujo de entrada en varios flujos concurrentes. Los nodos de bifurcación se introdujeron para admitir el paralelismo en las actividades. En comparación con UML 1.5, los nodos de bifurcación de UML 2.0 modelan el paralelismo sin restricciones. [1]


![fork con una entrada y 3 salidas](https://www.uml-diagrams.org/activity-diagrams/activity-fork.png)


**Rombo de decisión** - un nodo de decisión es un nodo de control que acepta tokens en una o dos puntos entrantes y selecciona un punto saliente de uno o más flujos salientes. Los nodos de decisión se introdujeron en UML para admitir condicionales en las actividades. [1]


![nodo de decisión con 2 salidas](https://www.uml-diagrams.org/activity-diagrams/decision-binary.png)


![nodo de decisión con 3 salidas](https://www.uml-diagrams.org/activity-diagrams/decision-ternary.png)


**Unión** - el nodo de unión es un nodo de control que cuenta con múltiples puntos entrantes y un saliente, y se utiliza para sincronizar flujos concurrentes entrantes. Los nodos de unión se introducen para admitir el paralelismo en las actividades.[1]


![nodo union](https://www.uml-diagrams.org/activity-diagrams/activity-join.png)


**Fase 2: Modelado del Proceso de Compra**
-----
**UML** - El Lenguaje Unificado de Modelado (UML) fue creado para forjar un lenguaje de modelado visual común y semántica y sintácticamente rico para la arquitectura, el diseño y la implementación de sistemas de software complejos, tanto en estructura como en comportamiento. UML tiene aplicaciones más allá del desarrollo de software, p. ej., en el flujo de procesos en la fabricación.[2]


![uml realizado](https://i.ibb.co/NHtT2P3/UML-drawio.png)


-   Justificación del uso de los nodos de sincronización.
Lo he utilizado dos veces. Primera vez para comprobar que sesión es valida y producto hay en stock. Lo hago en paralelo para no obligar a usuario esperar mas de que se necesita. Y próximo uso de  sincronización es cuando el producto esta pagado y se esta formando factura, actualización de base de datos y envió de notificación al correo de usuario. Como son 3 procesos paralelos y no se necesita confirmación de uno para que otro puede funcionar pues se puede hacerlo a la vez y así ahorramos tiempo del usuario.


**Webgrafía**
[1] K. Fakhroutdinov, “UML activity diagram controls are activity nodes coordinating the flows between other nodes: initial node, flow final, activity final, decision, merge, fork, join..” Accessed: May 12, 2026. [Online]. Available: https://www.uml-diagrams.org/activity-diagrams-controls.html
[2] “Qué es el lenguaje unificado de modelado (UML),” Lucidchart. Accessed: May 12, 2026. [Online]. Available: https://www.lucidchart.com/pages/es/que-es-el-lenguaje-unificado-de-modelado-uml
