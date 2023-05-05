## golang project

# Prerequisites

golang latest version
make latest version

# Lifecycle

build:    compile the source code of the application to a binary named awesome-api.
run:     Run the application in background by executing the binary awesome-api, and write logs into a file named awesome-api.log.
stop:    Stop the application with the command kill XXXXX where XXXXX is the Process ID of the application.
clean:   Stop the application. Delete the binary awesome-api and the log file awesome-api.log.
test:    Check expected behaviour of the app.
lint:    Static linting on go files using golangci-lint.
help:    Shows this help messages.