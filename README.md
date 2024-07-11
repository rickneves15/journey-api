# Journey API

The Journey API is a helpful tool that makes it easy to manage group trip details. It helps you confirm participants, create activities, generate links, and share trip details with everyone. It's like a digital planner that keeps everything organized and ensures everyone is on the same page

## Initial Configuration

To configure the Journey API, you need to set up the following initial settings:
  
```bash
  cp .env.example .env
  yarn
  npx prisma migrate dev
  yarn dev
```

- **DATABASE_URL**: URL for the database connection
- **API_BASE_URL**: Base URL for the API endpoints
- **WEB_BASE_URL**: Base URL for the web application
- **PORT**: Port number for the server to listen on (default: 8888)
  
## Technologies and Libraries Used

The Journey API is built using the following technologies and libraries:

- **Fastify**: Fast and low overhead web framework for Node.js
- **Zod**: Library for schema validation
- **Prisma**: Database toolkit and ORM for Node.js
- **Dayjs**: Library for date and time manipulation

## Routes

- [x] Confirm participant (`GET /participants/:participantId/confirm`);
- [x] Confirm participant (`GET /trips/:tripId/confirm`);
- [x] Create activity (`POST /trips/:tripId/activities`);
