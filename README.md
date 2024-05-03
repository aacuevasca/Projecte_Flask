## Com instalar un entorn virtual

Abans de començar a treballar, hem de crear un entorn virtual en el que treballar.  Per això, obrirem la terminal del Visual Code i executarem el seguent:

- Linux: 
	- ``python3 -m venv .venv

- Windows:
	- ``python -m venv .venv

Aixó ens instala el entorn virtual a la carpeta on ens trobem. Ens he d'asegurar de que es aizi perque si no ens donara problemes més endavant. Fet aixó, aurem d'activar-lo.

- Linux:
	- ``source .venv/bin/activate
	
- Windows:
	- ``.venv\Scripts\activate

Si ho hem fet bé, veurem el seguent prompt.
**![](https://lh7-us.googleusercontent.com/LELXzxsE9YEzk-sA3Rafrq_kWwms3tdJJ32rwqf9tV1k8moaFW4bpotk3D3qoyggAw-EmpN42R3k7mD7Yw89vpd3tfUYGQ6kzyCPqdRJPqzkkMtHX49dLYQMba1mJW97XYR3VHN-fYPtOcrvJ8d8JHY)

Ara ja podem instalar els paquets necessaris per el projecte, Flask i Feedparser. Per fer-ho, escriurem a la terminal un 'pip install'.

- ``pip install flask
- ``pip install feedparser

Amb aixó ya tenim instalar l'entorn virtual. I si volem sortir escriurem:

- deactivate
## Com iniciar l'aplicatiu

1. Assegura't d'haver configurat l'entorn virtual com es descriu més amunt. 
2. A la terminal, assegura't d'estar a l'arrel del projecte. 
3. Executa la següent comanda per iniciar l'aplicació:
```
python app.py
```
Això iniciarà l'aplicació i estarà disponible a http://localhost:5000.
## Mode d'Ús

L'aplicació pot funcionar en dos modes diferents:
### Mode Remot

En aquest mode, l'aplicació obté les dades directament des de la web de La Vanguardia.

Per a usar el mode remot, no es requereix cap configuració addicional.
### Mode Local

En aquest mode, l'aplicació utilitza un arxiu XML descarregat localment per a obtenir les dades.

Per a usar el mode local, segueix aquests passos:

1. Descàrrega l'arxiu XML des d'URL de l'arxiu XML.
2. Col·loca l'arxiu descarregat en l'arrel del projecte, al costat d'app.py.

Una vegada seleccionat el mode d'ús, l'aplicació funcionarà segons la configuració proporcionada.
## Detener la Aplicación
Per aturar l'aplicació, simplement prem Ctrl + C a la terminal on s'està executant l'aplicació.
## Recursos Adicionals
- Documentació de Flask
- Documentació de [Entorns Virtuals a Python](https://docs.python.org/3/library/venv.html)