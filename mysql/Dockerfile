# Use the official MySQL image from the Docker Hub
FROM mysql:latest

# Set environment variables for MySQL
ENV MYSQL_DATABASE=MYUsers
ENV MYSQL_ROOT_PASSWORD=1nd1a

# Expose port 3306 for MySQL
EXPOSE 3306

# Copy initialization scripts into the container
# All scripts in /docker-entrypoint-initdb.d/ will be executed during container startup
COPY ./sql-scripts/ /docker-entrypoint-initdb.d/


# FROM mysql:latest
# # Add a database
# ENV MYSQL_DATABASE=MYUsers
# ENV MYSQL_ROOT_PASSWORD=1nd1a
# ENV MYSQL_HOST=127.0.0.1
# EXPOSE 3306
# Add the content of the sql-scripts/ directory to your image
# All scripts in docker-entrypoint-initdb.d/ are automatically
# executed during container startup
# COPY ./sql-scripts/ /docker-entrypoint-initdb.d/
