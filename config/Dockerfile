FROM ghost:0.9.0
RUN npm install ghost-cloudinary-store && mkdir content/storage && cp -r node_modules/ghost-cloudinary-store content/storage/ghost-cloudinary-store
COPY ./config.js /var/lib/ghost/config.js
HEALTHCHECK CMD curl --fail http://localhost:2368/ || exit 1
