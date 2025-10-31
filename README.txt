DealX - The Campus Reuse Hub (Premium Ready-to-deploy)

Quick deploy summary:
1. Push this project to a new GitHub repo (root files as-is).
2. On Render: New -> Web Service -> connect the repo.
   - Build command: npm install
   - Start command: npm start
   - Health check path: /healthz
3. In Render service -> Environment add these variables:
   DATABASE_URL = your_postgres_internal_url
   CLOUDINARY_CLOUD_NAME = dj1ldcjda
   CLOUDINARY_API_KEY = 768128458791586
   CLOUDINARY_API_SECRET = <your_cloudinary_secret>
   PORT = 10000
4. Deploy -> Manual Deploy -> Deploy latest commit.
5. Test: open site, add listing (image uploads to Cloudinary), check listings.
