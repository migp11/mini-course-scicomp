# Herramientas

**Datos**
- pandas, polars, dask, pyarrow, xarray

**Modelado**
- numpy, xarray, scipy  

**Visualización**
- seaborn, matplotlib  

**Machine learning**
- scikit-learn, statsmodels  

**Entorno**
- Jupyter notebooks / JupyterLab

**Simulaciones**
- EMEWS, episim, epicommute, repast, netlogo

# Datasets

## Dataset Movilidad (MITMA v1) España
Este conjunto de datos contiene agregaciones diarias de los datos horarios proporcionados por MITMA, agregadas a diferentes niveles de resolución espacial.

**Maestra 1**: Matriz Origen-Destino para la capa de movilidad, con resolución horaria. Cada entrada incluye una fecha y un periodo horario (el intervalo entre dos horas consecutivas), las zonas de origen y destino, y el número de viajes entre el origen y el destino. Las zonas de origen y destino corresponden a geometrías de la capa de movilidad de MITMA, y también se registran los viajes internos (dentro de la misma capa de origen y destino).

**Maestra 2**: Matriz de viajes por persona en cada área de movilidad, con datos diarios. Este indicador informa sobre el comportamiento de movilidad diario de la población. Para cada fecha y zona de la capa de movilidad de MITMA, el indicador muestra cuántas personas han realizado 0, 1, 2 o más de 2 viajes. Si bien el indicador no proporciona el destino de los viajes, sí tiene en cuenta la proporción de personas que realizan al menos un viaje o ninguno, así como la población total estimada en esa zona para la fecha indicada (considerando como población a las personas que pernoctan en la zona en esa fecha).
Source: [https://www.transportes.gob.es/ministerio/proyectos-singulares/estudios-de-movilidad-con-big-data/estudios-de-movilidad-anteriores/covid-19]()

## Dataset COVID-19 España
Descripción: Datos desde el inicio de la pandemia, para todas las edades, hasta el 28 de marzo de 2022. Número de casos, número de hospitalizaciones, número de ingresos en UCI y número de defunciones por sexo, edad y provincia de residencia.
Source: [https://cnecovid.isciii.es/covid19/#documentaci%C3%B3n-y-datos]()

