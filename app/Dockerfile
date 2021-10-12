FROM node:8

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm ci --only=production

COPY . .

EXPOSE 8080
CMD [ "npm", "start" ]

LABEL Target="Dev" \
      owner="rob.wheeler@uk.zurich.com" \
      Department="ITSS-SecEng" \
      DataClassification="Internal"
