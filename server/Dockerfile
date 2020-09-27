# Trying out "alpine" OS for reduced image size
# Versions should be kept current with node and alpin lts distros
FROM node:14.11.0-alpine3.10

COPY package.json package.json
COPY package-lock.json package-lock.json

RUN npm install --only=prod 

COPY /dist /dist

CMD [ "node", "--experimental-modules", "/dist/index.js"]
