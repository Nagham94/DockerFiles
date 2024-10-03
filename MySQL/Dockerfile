# Use the official MySQL image from Docker Hub
FROM mysql:8.0

# Set environment variables for MySQL
ENV MYSQL_DATABASE=my_database \
    MYSQL_USER=user \
    MYSQL_PASSWORD=password \
    MYSQL_ROOT_PASSWORD=rootpassword

# Expose the default MySQL port
EXPOSE 3306

# Add a custom SQL script to initialize the database
# If you have custom SQL scripts, you can copy them to the container
COPY ./init.sql /docker-entrypoint-initdb.d/

# Set the command to run MySQL
CMD ["mysqld"]
