# tfmRNAseq
Repositorio TFM BioInfo 
# Objetivos del proyecto
TREM1 Triggering Receptor Expression of Mieloide Cells -> objetivo del proyecto es ver la señalización de esta molécula.
Se expresa en neutrófilos – células del sistema inmunitario.
Estos neutrófilos junto con los macrófagos y monocitos están incluidos en las células Mieloides.
A través de unos Dataset de cáncer de hígado de 169 pacientes, se intentará generar una serie de programas que analicen estos Dataset para ver como se expresan esos neutrófilos sobre una actividad inmunosupresora, que es negativa para el tumor. Buscamos la eliminación de esta actividad.
Impiden la actividad de las T-cells que son las células buenas que forman parte del sistema inmunitario.
De la población de células que podemos analizar con bulkRNAseq, se pretende pasar a los análisis sobre una sola célula, estudiar los distintos neutrófilos en una célula y hay es donde entra la señalización por TREM1.
Compararemos señales de firma entre Dataset sanos/controles  y Dataset con cancer.
	Perfil trascriptomico como se expresan estas células en el ADN.
	Cuando tienes cáncer expresas ese GEN -> TREM1 proteína y el gen del que proviene también se llama TREM1. 
TREM1 está asociado a cáncer de mama y también a su metástasis en cerebro, pulmón e hígado. 
Los neutrófilos de estos tejidos aumentan la expresión de TREM1.
Y esto esta relacionado con una menor supervivencia TREM1 survival.
Se sigue investigando sobre TREM1 en neutrófilos para afirmar que es patogénico y que favorece el crecimiento del tumor.
# Metodología
Análisis bioinformático con herramientas de bulkRNAseq y scRNAseq.
Uso de la herramienta web http://meta-cancer.cn:3838/scPLC/
Partimos de unos ficheros de pacientes con cancer hepático que han participado en el estudio del paper https://www.nature.com/articles/s41586-022-05400-x
Liver tumour immune microenvironment subtypes and neutrophil heterogeneity

En el contexto de ambientes tumorales, se ha estudiado el papel del TREM1 en la interacción entre el sistema inmunológico y el cáncer. La investigación ha sugerido que el TREM1 puede desempeñar un papel en la regulación de la respuesta inmunitaria en el microambiente de un tumor. Algunos estudios han demostrado que la sobreexpresión de TREM1 en los neutrófilos puede estar asociada con la promoción de la inflamación crónica y la supresión de la respuesta inmunitaria antitumoral.
Sin embargo, es importante tener en cuenta que la relación entre TREM1, los neutrófilos y los ambientes tumorales es un área de investigación activa, y se requieren más estudios para comprender completamente cómo este receptor puede influir en la respuesta inmunitaria contra el cáncer. Este estudio pretende con sus analisis de datos, procesado y visualizaciones poder reconfirmar las hipotesis de las que partimos.

# Descarga desde Drive los archivos spliteados proporcionados por la Universidad de Peking. 
https://drive.google.com/drive/folders/1mgqjO5ABV5mQxYRUbZEp4XVwCJ6BKW61 
Readme.txt
Download data
seu_A124.counts_anno.rds is the single cell RNA-seq data of 160 samples of human liver cancer. 
To avoid network interruption, we have splited seu_A124.counts_anno.rds into 10 small files. You can download them and run `cat seu_A124.counts_anno.rds.a* > seu_A124.counts_anno.rds` to generate the complete Rdata object.

# Generación de ficheros seu_A124.counts_anno.rds and seu_mouseLiverCancer.anno.rds
# Información del paper
Los datos de secuenciación sin procesar informados en este artículo se han depositado en el Archivo de Secuencia del Genoma del Centro Nacional de Datos Genómicos (Beijing, China) con el ID de BioProyecto PRJCA007744 . Los datos depositados y hechos públicos cumplen con las regulaciones del Ministerio de Ciencia y Tecnología de China. Para facilitar el uso de nuestros datos por parte de la comunidad de investigación en general, desarrollamos una herramienta interactiva basada en web ( http://meta-cancer.cn:3838/scPLC ) para analizar y visualizar nuestros datos unicelulares. Otros datos públicos utilizados en este estudio incluyen genomas de referencia para conjuntos de datos humanos ( https://asia.ensembl.org/ , GRCh38.p13) y de ratón ( https://asia.ensembl.org/ , GRCm39) y TCGA ( https: //portal.gdc.cancer.gov/ ). Los datos originales se proporcionan con este documento.

Disponibilidad de código
Los códigos utilizados en este estudio están disponibles en GitHub ( https://github.com/meta-cancer/scPLC ).

# Cluster HPC, Enviroment Conda e Instalación de entorno concreto.
Conda create
conda install
...
# 
