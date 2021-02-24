FROM registry.access.redhat.com/ubi8/nginx-118

ENV NGINX_VERSION=1.18

# Add application sources
ADD $NGINX_VERSION/test-app/nginx.conf "${NGINX_CONF_PATH}"
ADD $NGINX_VERSION/test-app/nginx-cfg/*.conf "${NGINX_CONFIGURATION_PATH}"
ADD $NGINX_VERSION/test-app/*.html ./

# Run script uses standard ways to run the application
CMD nginx -g "daemon off;"
