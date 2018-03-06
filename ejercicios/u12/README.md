# Ejemplos unidad 12: Negociación de contenidos

1. Copiamos los ficheros al `documentroot`/internacional de apache1.
2. Activamos la negociación de contenidos

		<Directory /var/www/apache1/intenacional>
    		Options +Multiviews
    	</Directory>	

3. Y porobamos, cambiando el idioma del navegado.

4. A continuación vamos a probar los type-map

		<Directory /var/www/apache1/intenacional>
			DirectoryIndex index.var
    		AddHandler type-map .var
    	</Directory>

5. Y volvemos a probar
