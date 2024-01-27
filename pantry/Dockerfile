FROM node:21.6.0-alpine3.19
ENV JAM_CONFIG_DIR=/jam-config
RUN mkdir /pantry
WORKDIR /pantry
COPY yarn.lock package.json /pantry/
RUN yarn
COPY . /pantry
EXPOSE 3001
CMD node ./bin/www
