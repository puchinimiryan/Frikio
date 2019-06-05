![alt text](/images/icon.png)



# Agradecimientos
En nombre de todos los organizadores les agradecemos enormemente su participación y los envitamos a ponerse en contacto de cara a la organización de futuras meetups mediante la suscripción al listado de misol:
https://listas.unam.edu.ar/cgi-bin/mailman/listinfo/misol


# Material de las charlas :
[“Carpeta slides_charlas”](https://gitlab.com/sergio08/mini_chall_fsm_2018/tree/master/slides_charlas)

# Ganador del Mini-Challenge
| Name  | Accuracy | 
| Facundo Dominguez  | 0.7643 | 

# Imágenes para el submit del Mini Challenge:
Si mejoraste alguno de los modelos, o tenés tu propio modelo usa el set de submit para generar tus predicciones y envialas como adjunto email de contacto para participar por los premios.

Agregamos un sel set de submit para aquellos que entrenaron con los csv en lugar de con las imagenes.

-  [submit para los entrenados con las imágenes](https://gitlab.com/sergio08/mini_chall_fsm_2018/blob/master/datasets/images/submit.tar.gz)
-  
- [submit para los entrenados con los csvs](https://gitlab.com/sergio08/mini_chall_fsm_2018/blob/master/datasets/submit_ParaLosEntrenadosCon%20elCSV.csv)




# Mini-Challenge "Mandar menos fruta"  - Free Software Meetup 2018

Esta competencia esta dirigida a aquellos participantes de la FSM 2018 que están interesados en dar sus primeros pasos en inteligencia artifical y machine learning. Y tiene como objetivo de complementar a nivel práctico las charlas de la FSM que se darán sobre dicha temática.

La competencia consiste en generar un clasificador automático que permita discriminar de la mejor manera posible entre 8 tipos de figuras dibujadas a mano, las cuales han sido obtenidas del proyecto de google labs "Quick Draw" (¿Lo conocés? , sino podes pegarle una mirada a este super interesante proyecto para ver de que se trata en:  https://quickdraw.withgoogle.com/data ). 



## Dataset
Con el objetivo de hacer las cosas un poco más sencillas, hemos generado un set de datos el cual está disponibilizado en su versión de imagen  (28 x 28 pixels, organizadas en carpetas llamdas con el nombre de la fruta en particular) o como una tabla en la que cada fila contienen los valores de cada uno de los pixeles (784 columnas, una por cada pixel más 1 columna con la correspondiente clase o categoría de fruta). Si querés podes usar este codigo en python (  [notebook](https://gitlab.com/sergio08/mini_chall_fsm_2018/blob/master/notebooks/gettingImmgesFromQuickDraw.ipynb) ) para bajarte más imagenes de cada categoría.


| Name  | Content | amount | Size | Link|
| --- | --- |--- | --- |--- |
| `train.tar.gz`  | Imagenes de entrenamiento  | 12800 |4.9 MBytes | [Download](https://gitlab.com/sergio08/mini_chall_fsm_2018/blob/master/datasets/images/train.tar.gz)|
| `train.csv`  | Set de entrenamiento vect  | 12800 |4.9 MBytes | [Download](https://gitlab.com/sergio08/mini_chall_fsm_2018/blob/master/datasets/train_12800.csv)|
| `test.tar.gz`  | Imagenes de testeo  | 1600 |0.6  MBytes | [Download](https://gitlab.com/sergio08/mini_chall_fsm_2018/blob/master/datasets/images/test.tar.gz)|
| `test.csv`  | Setde testeo vect  | 1600 |0.6  MBytes | [Download](https://gitlab.com/sergio08/mini_chall_fsm_2018/blob/master/datasets/test_1600.csv)|
| `submit.tar.gz`  | Imagenes para generar el submit final  | 1600|0  MBytes | [Download](https://gitlab.com/sergio08/mini_chall_fsm_2018/blob/master/datasets/images/submit.tar.gz)|
| `submit.csv`  | Set de submit alt para sulos entrenados con los csv | 1600|0  MBytes | [Download](https://gitlab.com/sergio08/mini_chall_fsm_2018/blob/master/datasets/submit_ParaLosEntrenadosCon%20elCSV.csv)|

## Categorías "Frutales"
Los distintos tipos de figuras seleccionadas corresponden a 8 tipos distintos de frutas : 

![alt text](/images/fruits.png)

## Reglas de la competencia y elección del mejor modelo 
Las reglas del juego son todas, podes usar el tipo de algoritmo,  herramientas y  métricas que prefieras. Un día antes de las charlas disponibilizaremos en el repo un nuevo set de imágenes para que generes predicciones usando tu mejor modelo y nos lo envies a un email que ya disponibilizaremos y eligiremos como ganador a aquel modelo que "mande menos fruta".  Los resultados de las distintas aproximaciones se discutiran y pondran en común durante la entrega de premios.

# Submit de resultados
Con el fin de evaluar los resultados, una vez habilitado el set de imagenes de submit, deberás realizar tus predicciones con el mejor modelo que hayas obtenido y deberas enviar un archivo .csv con el formato que se detalla debajo a un email que comunicaremos el día de las charlas, con el asunto:  Mini-ChallengeFSMM2018

Ejemplo del formato requerido para el submit:
Nombre_Apellido.csv

|image  | prediction |
| --- | --- |
|000a3728-eb5f-4db4-90cf-3d6f663f9e2f.jpeg |peanut|
|0071324c-384b-46c4-b57f-add46b67d08a.jpeg |apple|
|0081934a-f824-4bf7-b50c-26e89ca3dc0b.jpeg |pear|
|... |...|

O en el caso del submit para los entrenados a partir de csvs

|image  | prediction |
| --- | --- |
|1 |peanut|
|3|apple|
|5 |pear|
|... |...|



## Premios
Gran premio sorpresaaa!

## Ejemplos
Para ayudarte en estos primeros pasos en la carpeta /notebooks vas a encontrar notebooks de jupyter lab  para procesar y correr algoritmos básicos de machine learning y deep learning utilizando  keras en [R](https://gitlab.com/sergio08/mini_chall_fsm_2018/blob/master/notebooks/Examples_using_R.ipynb)  o [python](https://gitlab.com/sergio08/mini_chall_fsm_2018/blob/master/notebooks/Examples_using_Python.ipynb)  . Vas a poder usar estos scripts como base para mejorar tu propio modelo.


Otros herramientas y lugares donde encontrar más ejemplos e ideas:
- kaggle: https://www.kaggle.com/
- Pytorch : https://pytorch.org/tutorials/beginner/pytorch_with_examples.html
- Tensorflow: https://www.tensorflow.org/
- Mxnet: http://mxnet.incubator.apache.org/
- Caffe: http://caffe.berkeleyvision.org/
- Theano: http://www.deeplearning.net/software/theano/


## Contacto

![alt text](images/email.png)

## Install and running with R

Suggested alternative:
install Conda, create an environment with R essentials  (https://anaconda.org/r/r-essentials) and then run the example notebook using jupyter lab. 

Quick install and some tips at Linux:
1) download miniconda installer: 
>wget https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh
2) install
>bash Miniconda3-latest-Linux-x86_64.sh
3) Install supports for jupyter lab  (more details at "https://github.com/jupyterlab/jupyterlab")
>conda install -c conda-forge jupyterlab
4) create an environment in order to be used with R
>conda create --name py36R
5) open the environment and Install R-essentials (essentials bring with 80 DS packages tidyverse,shiny) 
>source activate py36R

>conda install -c r r-essentials 

>conda install nb_conda
6) Finally, open jupyter lab and run the notebook(.ipynb)

For more informations using install using another OS "https://conda.io/docs/user-guide/install/index.html"




## Install and running with Python

Suggested alternative: install Conda, create an environment with python and then run the example notebook using jupyter lab.

Quick install and some tips at Linux:

1) download miniconda installer:

wget https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh

2) install

bash Miniconda3-latest-Linux-x86_64.sh

3) Install supports for jupyter lab (more details at "https://github.com/jupyterlab/jupyterlab")

conda install -c conda-forge jupyterlab

4) create an environment (default Python 3.6.5)

conda create --name py36

5) open the environment and required packages

source activate py36

conda install -c numpy scipy matplotlib pandas scikit-learn ipython nbconvert tensorflow keras nb_conda opencv

conda install nb_conda 6) Finally, open jupyter lab and run the notebook(.ipynb)

For more informations using install using another OS "https://conda.io/docs/user-guide/install/index.html"


