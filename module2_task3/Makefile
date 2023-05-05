build:	## Builds the API binary file using go
	make lint
	go build

run:	## Runs the built binary and send everything to awesome.log
	./awesome-api >./awesome.log 2>&1 &

stop:	## Terminates the execution of awesome-api
	kill $(shell pgrep awesome-api)

clean:	## Removes binary and logs
	-make stop
	-rm ./awesome-api awesome.log coverage*

test:	## Tests API using go test
	make unit-tests
	make integration-tests

lint:	## Lints all the go files using golangci-lint
	golangci-lint run

unit-tests:	## Runs implemented unit test using go test
	go test -v -short -coverprofile=coverage-units.out

integration-tests:	## Runs integration test using go test
	go test -v -coverprofile=coverage-integrations.out

help:	## Show this help message
	@fgrep -h "##" $(MAKEFILE_LIST) | fgrep -v fgrep | sed -e 's/\\$$//' | sed -e 's/##//'