FROM node:10.15.1
LABEL maintainer “Paladin and Archer”

ENV PORT 3000

WORKDIR /home/app

COPY scripts/package.json ./package.json
COPY scripts/start.sh ./start.sh
RUN chmod 777 ./start.sh
RUN chmod 777 ./package.json
RUN chmod 777 .

USER node

EXPOSE 3000

CMD /home/app/start.sh
