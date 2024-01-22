FROM node:lts-alpine
WORKDIR /app
COPY package*.json .
RUN npm install
COPY . .
CMD ["npm", "start"]

# docker build -t myreact .
# docker run -it -p 3000:3000 --name react myreact
# docker run -it -p 3000:3000 --mount type=bind,src="$(pwd)",dst=/app myreact
# docker container run --rm -it -p 3000:3000 --mount dst=/app/node_modules --mount type=bind,src="$(pwd)",dst=/app myreact

# Si windows
# docker run -it -p 3000:3000 -e WATCHPACK_POLLING=true --mount type=bind,src="$(pwd)",dst=/app myreact
