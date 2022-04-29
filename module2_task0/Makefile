build: ##Compilacion de codigo fuente
	go build -o awesome-api
run: ##Ejecucion del binario awesome-api
	./awesome-api >./awesome.log 2>&1 &
stop: ##Detenido de aplicacion con comando kill
	kill $$(pgrep awesome-api)
clean: ##Borrado del binario awesome-api y del log
	rm awesome*
test: ##Comprobar el funcionamiento esperado de la app
	curl http://localhost:9999
	curl http://localhost:9999/health
help: ##Despliega esta ayuda
	@grep -E '([a-zA-Z]+:)\s(##)(.+)' $(MAKEFILE_LIST) | sed 's/##//'
