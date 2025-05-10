# Stage 1: Build
FROM node:18-slim AS builder

WORKDIR /app
COPY . .

# Clean up potentially corrupted dependencies
RUN rm -rf node_modules package-lock.json

# Install fresh deps and build
RUN npm install
RUN npm run build

# Stage 2: Serve via Nginx
FROM nginx:alpine
COPY --from=builder /app/dist /usr/share/nginx/html
COPY ./nginx.conf /etc/nginx/conf.d/default.conf

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
