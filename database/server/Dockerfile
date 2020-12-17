FROM mysql:5.7

ENV MYSQL_ROOT_PASSWORD=example
ENV MYSQL_DATABASE=company_a
ENV MYSQL_USER=vorapod
ENV MYSQL_PASSWORD=password

COPY ./dump /docker-entrypoint-initdb.d

VOLUME [ "/docker-entrypoint-initdb.d" ]

CMD ["mysqld","--default-authentication-plugin=mysql_native_password","--lower_case_table_names=1"]