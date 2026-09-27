# Tool Library API
This project is a tool lending library API where the whole library of tools can be viewed with their attributes, a specific tool can be found, a tool can be created, a tool's field can be replaced if needed, or a tool can be removed.

Live: https://cpan212-lab2-melissa-paredes.onrender.com/api/tools 

## Run it

```bash
npm install
cp .env.example .env
npm run dev
```

The API runs at http://localhost:4000. Set `PORT` in `.env` to use a different port.

## Routes

| Method | Path | What it does |
|---|---|---|
| GET | `/api/tools` | Every tool. `?category=garden` keeps only one category |
| GET | `/api/tools/:id` | One tool, or 404 |
| POST | `/api/tools` | Create a tool (201), or 400 with the invalid fields |
| PUT | `/api/tools/:id` | Replace a tool's fields (200), 400 or 404 |
| DELETE | `/api/tools/:id` | Remove a tool (204), or 404 |

## Testing

```bash
npm run check
```

This tries every route and prints which checks pass.

## AI use

AI was used to learn about routing, middleware, and express handling. I am someone who learns well when I have lots of examples to refer to. I took the notes from Week 3 and asked google gemini to make me concise notes and provide learning examples so that I can complete the lab by myself. 
