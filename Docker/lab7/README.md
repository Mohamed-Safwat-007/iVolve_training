Lab 7: Docker Volume and Bind Mount with Nginx
• Create nginx_logs volume to persist Nginx logs and verify it in the default
volumes path.
• Create a directory nginx-bind/html to serve a custom HTML file from your host
machine.
• Create index.html file with “Hello from Bind Mount” syntax in nginx-bind/html
directory.
• Run Nginx container with the following:
 Volume for /var/log/nginx
 Bind Mount for /usr/share/nginx/html
• Verify Nginx page by running curl command from your local machine.
• Change in the index.html file in your local machine then verify Nginx page again.
• Verify logs are stored in the nginx_logs volume.
• Delete the volume.

