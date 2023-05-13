# Awesome Website

Project for DevOps on Holberton School

## Prerequisites

GoHugo on extended version - v0.84 or above
make - v3.81 or above

## Lifecycle

build: Generate the website from the markdown and configuration,
files in the directory dist/ and compile the source code of,
the application to a binary named awesome-api
clean: Cleanup the content of the directory dist/,
the binary awesome-api and the log file awesome-api.log,
post: Create a new blog post whose filename and title,
come from the environment variables POST_TITLE and POST_NAME.
run: Run the application in background by executing,
the binary awesome-api, and write logs into a file,
named awesome-api.log stop: Stop the application with,
the command kill XXXXX where XXXXX is the Process,
ID of the application.
test: Check expected behaviour of the app lint: Static,
linting on go files using golangci-lint unit-tests: execute,
(successfully) the Golang unit tests integration-tests: execute,
the Golang integration tests check: Markdown linting on,
syntax and dead links validate: should validate the,
file ./dist/index.html by using the command line Holberton’s,
W3C Validator help: Shows this help message

## Build Workflow

Does static linting and build both website and API binary
