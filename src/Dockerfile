FROM  mhart/alpine-node:10  as builder

RUN apk --no-cache add \
    git

RUN git clone https://github.com/ExcitableAardvark/monerod_exporter.git /etc/monerod-exporter

WORKDIR /etc/monerod-exporter

RUN npm install

ENTRYPOINT [ "node" ]
CMD [ "index.js" ]