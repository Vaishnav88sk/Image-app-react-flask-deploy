# FROM python:3.8

# WORKDIR /app

# EXPOSE 5050

# COPY Pipfile Pipfile.lock ./


# # RUN pip install pipenv
# RUN pip install --no-cache-dir pipenv
# RUN pipenv lock --requirements > requirements.txt
# RUN pip install -r requirements.txt

# COPY . ./

# CMD ["python", "main.py"]

FROM python:3.8

# Set the working directory inside the container
WORKDIR /app

# Expose the port the app runs on
EXPOSE 5050

# Copy dependency management files
COPY Pipfile Pipfile.lock ./

# Install pipenv and dependencies
RUN pip install --no-cache-dir pipenv && \
    pipenv install --system --deploy

# Copy the rest of the application code
COPY . ./

# Command to run the application
CMD ["python", "main.py"]
