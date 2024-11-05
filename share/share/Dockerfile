# Use the official Apache image from Docker Hub
FROM httpd:2.4

# Install necessary packages
RUN apt-get update && apt-get install -y \
    git \
    && rm -rf /var/lib/apt/lists/*

# Clone the GitHub repository
RUN git clone https://github.com/VSNINT/GamutElectronics.git /usr/local/apache2/htdocs/

# Set the document root directory to the cloned repo's content
WORKDIR /usr/local/apache2/htdocs

# Expose port 80 for the HTTP server
EXPOSE 80


