FROM node:10-alpine as build
WORKDIR /app
COPY ./package.json /app
RUN npm install
COPY . /app
RUN npm run build --prod --outputPath=./dist/tlcfront

FROM bunkerity/bunkerized-nginx
# EXPOSE 8080
COPY --from=build /app/dist/tlcfront /www