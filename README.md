# Mars Terraformálása – Erőforrás Board

Egy egyszerű React + Supabase alapú webalkalmazás erőforrások kezelésére (Mars terraformálása játékhoz).

## Fő funkciók
- Erőforrások: money, steel, titanium, plant, energy, heat
- +1, -1, +5, -5 gombok minden erőforráshoz
- Termelési érték szerkesztése (+/-1, +/-5)
- "Termelés" gomb, ami hozzáadja a termelést a készlethez
- Automatikus termelés (5 másodpercenként)
- Mentés Supabase adatbázisban a session ID alapján
- Partner tábla megnyitása egy partner ID megadásával

## Telepítés (lokálisan)
1. Másold a `.env.example` fájlt `.env`-re és állítsd be a Supabase adatokat.
2. `npm install`
3. `npm run dev`

## Supabase
- A `supabase/schema.sql` fájl tartalmazza a szükséges SQL-t a `boards` tábla létrehozásához.
- Teszteléshez engedélyezheted a RLS policy-ket lazán, de éles környezetben állíts be auth-ot és megfelelő policy-ket.

## Deploy
- Build: `npm run build`
- Host: Vercel vagy Netlify (mindkettő ingyenes csomagot kínál).