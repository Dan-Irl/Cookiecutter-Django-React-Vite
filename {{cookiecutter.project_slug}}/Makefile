#################################################################################
# GLOBALS                                                                       #
#################################################################################

PROJECT_NAME = {{cookiecutter.project_slug}}
PYTHON_VERSION = cookiecutter.python_version
PYTHON_INTERPRETER = django-react

#################################################################################
# COMMANDS                                                                      #
#################################################################################


#################################################################################
# Local development

# Build for local development
.PHONY: build-local
build-local:
	docker compose -f local.yml build

# Run for local development
.PHONY: run-local
run-local:
	docker compose -f local.yml up

# Down for local development
.PHONY: down-local
down-local:
	docker compose -f local.yml down

#################################################################################
# Production

# Build for production development
.PHONY: build-production
build-production:
	docker compose -f production.yml up

# Run for production development
.PHONY: run-production
run-production:
	docker compose -f production.yml build

# Down for local development
.PHONY: down-production
down-production:
	docker compose -f production.yml down

