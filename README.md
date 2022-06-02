# Polisognograma
Analisis y creación de modelos, para la detección de las fases del sueño.  


Tenemos dos fuentes de datos:  

* Los datos del aula virtual son del mismo hospital de portugal, pero son un .mat que ya esta más o menos procesado, no los vamos a usar para nada por ahora.   
* Otros que son de un hospital de Portugal ([link](https://sleeptight.isr.uc.pt/?page_id=48)) y tiene diferentes tipos:  
    * Datos simples de gente con patologías.  
    * Datos dobles para ver la varianza de un mismo individuo.  
    * Datos de pacientes de control.  
    
    
Vamos a usar una librería para cargar y manejar datos de señales medicas estilo ECG... El paquete es MNE ([link](https://mne.tools/stable/auto_tutorials/index.html)). Eso para cargar las señales médicas, filtros y tal. Luego una librería específica para el procesado de señales de polysognograma es Yasa ([link](https://raphaelvallat.com/yasa/build/html/index.html)). Concretamente vamos a seguir el _Quickstart_ de la documentación ([link](https://raphaelvallat.com/yasa/build/html/quickstart.html)).  

Otras librerías que podrían ser útiles para la el tratamiento de señales son:  
* Scipy ([link](https://docs.scipy.org/doc/scipy/tutorial/signal.html)).  
* Pywt ([link](https://pywavelets.readthedocs.io/en/latest/))



**Presentacion:**

https://docs.google.com/presentation/d/1LK3ThTByrCmwiiCd3abrP1YpBPSAGgkoRKZa0zfAwXM/edit?usp=sharing



**TODO:**

El objetivo es hacer el _Quickstart_ y luego entrenar un clasificador lo más sencillo posible para que nos haga la clasificación atendiendo a alguna característica de los segmentos de 30 segundos que vayamos sacando de las señales.
