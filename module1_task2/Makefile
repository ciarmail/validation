build: ##Creacion de carpeta 'dist' y generacion de sitio web en esta carpeta
	mkdir ./dist
	hugo server -d ./dist/
clean: ##Borrado del sitio web generado en la carpeta 'dist'
	rm -r ./dist/*
post: ##Creacion de nuevo post who-we-are y reemplazo del titulo con el comando 'sed'
	hugo new 'posts/$(POST_NAME).md'
	sed -i 's/Who Are We/$(POST_TITLE)/' content/posts/$(POST_NAME).md
#	sed 's/false/true/' posts/$POST_NAME.md
help: ##Despliega esta ayuda
	@grep -E '([a-zA-Z]+:)\s(##)(.+)' $(MAKEFILE_LIST) | sed 's/##//'