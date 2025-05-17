FROM almalinux:8

# Install nginx
RUN yum install -y nginx && yum clean all

# Replace the default index.html
RUN rm -f /usr/share/nginx/html/index.html
RUN echo "<h1>Hello, I am from APP-1</h1>" > /usr/share/nginx/html/index.html

# Start Nginx in the foreground
CMD ["nginx", "-g", "daemon off;"]