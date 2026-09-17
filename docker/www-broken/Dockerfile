FROM nginx:alpine
LABEL org.opencontainers.image.source=https://github.com/fase29/kind-canary-demo
COPY /src/index.html /usr/share/nginx/html/index.html
# healthz deliberately NOT copied -> /healthz returns 404
# pods still pass the readiness probe on "/", so they go Ready
