# Git básico
Una aproximación a los conceptos básicos de Git

### Alcance
- Se presentan los conceptos básicos de Git para entender la metodología de control de versiones mediante esta tecnología.
- La información que aquí se vierte sobre Git es independiente del cliente que se utilice (Gráfico, Consola, etc...). Esa es una de las razones por ls que no se incluyen líneas de código o comandos de terminal con la finalidad de que estos sean aprendidos. 
- El fin último es comprender los conceptos elementales y aprender el flujo de trabajo básico para iniciarse en la práctica del control de versiones.
- No se incluye aquí información sobre la instalación de Git en las diferentes plataformas, cuestión que puede resuelve fácilmente siguiendo la información disponible en la [web de Git] [1]


—-

### ¿Qué es Git?
Git es una herramienta de control de versiones (VCS) *distribuida*, es decir, un sistema en el que cada cliente replica (clona) el repositorio de trabajo completo.

#### Beneficios del control de versiones
- Posibilidad de recuperar versiones anteriores de un archivo modificado como parte de un proceso de diseño.
- Regresar a una versión anterior del conjunto de documentos de un proyecto.
- Comparar versiones de un archivo a lo largo del tiempo.
- Verificar la autoría de un determinado cambio.
- Finalmente, usando un VCS tendrás una copia de respaldo de la documentación de un proyecto y se minimizará el riesgo de pérdida definitiva de un archivo.

---


### Características fundamentales de Git
- Los cambios se registran realizando copias instantáneas de cada archivo no registrando únicamente las diferencias.
- Las operaciones son (casi) todas locales reduciendo el tiempo de trabajo al no consumir en cada modificación  recursos de red.
- Todo es verificado mediante *check-sum*, lo cual hace imposible el supuesto de que un documento sea modificado sin que la herramienta identifique dicho cambio. Esta suma de comprobación es generada mediante el hash SHA-1
- Generalmente el sistema sólo añade información, lo que hace de la herramienta un sistema robusto frente al riesgo de pérdida de información 

#### Los tres estados
Los archivos en Git pueden encontrarse en alguno de estos tres estados:
- Committed (o confirmado): significa que las modificaciones están almacenadas de forma segura en la base de datos local.
- Modified (o modificado): Existes modificaciones que no han sido confirmadas.
- Staged (o preparado): el archivo modificado ha sido marcado para el próximo commit (confirmación)
#### Secciones principales de un proyecto Git
- Working directory
- Staging directory
- Git directory

#### Flujo de trabajo básico 
1. Modificación de archivos en el directorio de trabajo. *Status* resultante: **Modified**.
2. Preparación de archivos añadiéndolos al Staging directory. *Status* resultante: **Staged**.
3. Confirmación de cambios (commit). *Status* resultante: **Committed**


---
### Bibliografía y recursos
- [Pro Git book](https://git-scm.com/book/en/v2)
- [1]: https://git-scm.com/downloads
