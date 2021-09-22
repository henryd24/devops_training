FROM nginx:alpine
 # use a volume is mor efficient and speed that filesystem
VOLUME /tmp
RUN rm -rf /usr/share/nginx/html/*
COPY nginx.conf /etc/nginx/nginx.conf
COPY dist /usr/share/nginx/html/dist
#expose app and 80 for nginx app
EXPOSE 80 81
CMD ["nginx", "-g", "daemon off;"]
