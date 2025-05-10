## 🛠 Getting Started

Follow these steps to run the project locally with Docker, PostgreSQL, and Prisma:

### 1. Clone the repository

```bash
git clone https://github.com/your-username/your-project.git
cd your-project
2. Install dependencies
Use your preferred package manager:

bash
Copy
Edit
npm install
# or
yarn
# or
pnpm install
# or
bun install
3. Configure environment variables
Create a .env file in the root directory by copying the example:

bash
Copy
Edit
cp .env.example .env
Update the variables if needed. If you're using Docker, the default DATABASE_URL should already work.

4. Start PostgreSQL with Docker
Spin up the database container:

bash
Copy
Edit
docker-compose up -d
This will start a PostgreSQL database in the background.

5. Run Prisma migrations and seed the database
Apply the schema and insert seed data:

bash
Copy
Edit
npx prisma migrate dev --name init
npx prisma db seed
6. Start the development server
Run the app locally:

bash
Copy
Edit
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
Open your browser and navigate to:

👉 http://localhost:3000
