FROM node

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 3333

CMD ["node", "app.js"] 

# Step 1 ✅ cached

# Step 2 ✅ cached (package files didn’t change)

# Step 3 ✅ cached (npm install reuses cache)

# Step 4 ❌ re-run because COPY . . now sees a change

# Step 5 ❌ re-run