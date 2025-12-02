# School-Management-System
You can git clone repo-https-name or download zip file
after this you'll need to check if you have Node, DockerDescktop
if no, then install both
then you'll need to go to Clerk to get your public & private API_KEY


after done all of that you'll go the to your project Dir
enter:
- docker-compose up -d

then you'll need to generate prisma and setting up migrations
with these command:

Option A — Run command directly
- docker-compose exec app npx prisma generate
- docker-compose exec app npx prisma migrate dev --name init

Option B — Enter container shell first
- docker-compose exec app bash <br>
Now you are inside container, prompt looks like: /app
- npx prisma generate
- npx prisma migrate dev --name init
exit

Finished: you can now go to browser and enter localhost:3000
