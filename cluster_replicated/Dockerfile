FROM clickhouse/clickhouse-server:23.8.11.28
ENV TZ=Asia/Shanghai
RUN echo "${TZ}"
RUN apt update \ 
&& apt install -y tzdata \ 
&& echo "${TZ}" > /etc/timezone \ 
&& ln -sf /usr/share/zoneinfo/${TZ} /etc/localtime \ 
&& rm -rf /var/lib/apt/lists/*
