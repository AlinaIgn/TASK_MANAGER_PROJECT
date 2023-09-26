# Define the Python interpreter and manage.py command
PYTHON = python3
MANAGE = $(PYTHON) manage.py

# Development server
runserver:
	$(MANAGE) runserver

# Apply database migrations
migrate:
	$(MANAGE) makemigrations
	$(MANAGE) migrate

# Create a superuser
createsuperuser:
	$(MANAGE) createsuperuser

# Run tests (customize the test target)
test:
	$(MANAGE) test task_manager

# Clean up pycache files
clean:
	find . -name "*.pyc" -exec rm -f {} \;
	find . -name "__pycache__" -exec rm -rf {} \;

# Start the Django shell
shell:
	$(MANAGE) shell



.PHONY: runserver migrate createsuperuser test clean shell
