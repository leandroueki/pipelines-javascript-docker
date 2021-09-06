FROM node:latest

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm ci --only=production

COPY . .

LABEL Target="Prod" \
      owner="leandro.ueki@zurich.com" \
      Department="ITSS-Architecture" \
      DataClassification="Internal" \
      PlanningIT="54321"
