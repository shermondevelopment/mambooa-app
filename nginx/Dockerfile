FROM nginx:1.15.0

# REMOVE A CNFIGURAÇÃO PADRÃO DO NGINX
RUN rm /etc/nginx/conf.d/default.conf

# COPIANDO A CONFIGURAÇÃO QUE VAMOS CRIAR
COPY nginx.conf /etc/nginx/conf.d
