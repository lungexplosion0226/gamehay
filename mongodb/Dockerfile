FROM mongo:4.4.6
RUN echo "password" > /keyfile \
    && chmod 600 /keyfile \
    && chown 999 /keyfile \
    && chgrp 999 /keyfile
CMD ["--bind_ip_all", "--keyFile", "/keyfile", "--replSet", "rs0", "--port", "27017"]


# mongo -u admin -p BTovsgJZ2Hfxr18 (username và password trong file config .env)
# rs.secondaryOk()
# rs.initiate()