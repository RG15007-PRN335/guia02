FROM postgres:9.6.3-alpine
MAINTAINER Angel Eduardo Ruiz Gonzalez “aeduardoruizg@gmail.com”
COPY posts_v2.sql /docker-entrypoint-initdb.d/
ENV PGDATA /var/lib/postgresql/data 
VOLUME /var/lib/postgresql/data 
ENTRYPOINT ["/docker-entrypoint.sh"] 
EXPOSE 5432
CMD ["postgres"]
