FROM node:16-alpine3.18

# Install dependencies
RUN apk --no-cache add \
    nano \
    zip \
    unzip \
    curl

# Change current user
USER node

EXPOSE 5173

# https://github.com/vitejs/vite/discussions/3396
CMD ["sh", "-c", "npm install && npm run dev -- --host"]