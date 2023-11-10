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

