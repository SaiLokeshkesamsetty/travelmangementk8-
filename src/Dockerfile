FROM nginx:stable-alpine

# Use prebuilt static files if available. Adjust the folder name below if your
# build output directory is `dist` instead of `.dist`.
COPY .dist/ /usr/share/nginx/html

# Custom nginx config for SPA routing (keeps existing config)
COPY nginx.conf /etc/nginx/conf.d/default.conf

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
