Word Battler — Mobile-first Word Mini-Games (Next.js + Redis + NextAuth)

Setup

1. Copy env and set values:

```
cp .env.example .env.local
```

Required variables:

- NEXTAUTH_SECRET
- GOOGLE_CLIENT_ID / GOOGLE_CLIENT_SECRET (optional)
- REDIS_URL (default redis://localhost:6379)

2. Install deps:

```
npm install
```

3. Run dev:

```
npm run dev
```

Key routes

- /auth/signup — email+password signup
- /auth/signin — credentials or Google
- /hub — game hub
- /games/wordle-timer — singleplayer MVP

API stubs

- POST /api/game/single/wordle-timer/start
- POST /api/game/single/wordle-timer/submit
- GET /api/words/[length]
- GET /api/leaderboard/[game]
# word-battle
