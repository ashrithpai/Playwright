FROM node:alpine
COPY . /app
WORKDIR /app
RUN npm install -D @playwright/test
RUN npx playwright install webkit

# Run playwright test
CMD [ "npx", "playwright", "test", "--reporter=list" ]