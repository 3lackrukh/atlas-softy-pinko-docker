# Use the latest Ubuntu image as the base
FROM ubuntu:latest

# Update APT and upgrade all existing packages
RUN apt-get update
RUN apt-get upgrade -y

# Remove unnecessary files after installation
RUN apt-get clean && \
    rm -rf /var/lib/apt/lists/*

# Set the working directory inside the container
WORKDIR /task0

# Copy the entrypoint script into the container
COPY ./entrypoint.sh /task0/entrypoint.sh

# Make the entrypoint script executable
RUN chmod +x /task0/entrypoint.sh

# Run the entrypoint script when the container starts
ENTRYPOINT ["/task0/entrypoint.sh"]
