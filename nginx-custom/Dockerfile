FROM nginx:latest

USER root

RUN apt-get update && \
    apt-get install -y unzip curl python3 python3-pip && \
    pip3 install awscli && \
    apt-get clean

# Ensure nginx folders exist
RUN mkdir -p /usr/share/nginx/html

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
