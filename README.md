# Total 22

Arcade football made for playing with people in the room.

Pick up a keyboard or controller, take control of a player, and play 11v11 matches where every other player has their own AI brain. Build a squad, call a room code, or just kick off.

## Run locally

```sh
pnpm install
pnpm dev
```

Open [http://localhost:5173](http://localhost:5173).

For a LAN game, run the server on one computer and have everyone open:

```text
http://<host-ip>:5173
```

Then join the same four-letter room code.

## Modes

- **Quick Match** — set the teams and kick off.
- **Draft Mode** — build an XI from the player market.
- **Gamble Mode** — roll for your squad and work with what you get.
- **Training Ground** — learn the controls with the pitch to yourself.
- **Online Play** — host or join a room with friends.

## Controls

| Action | Keyboard | Controller |
| --- | --- | --- |
| Move | `WASD` | Left stick |
| Sprint | `Shift` | `LT` |
| Kick | Hold and release `Space` | Pull and release `RT` |
| Switch player | `E` | `A` |
| Feint / tackle | `K` | `B` |
| Croqueta / slide | `J` | `X` |
| Rainbow / barge | `L` | `Y` |
| Controls card | `C` | Select |

Kicks reward timing. Hold too long and the shot fizzles. Slides from behind are fouls. Skill moves depend on positioning, not random button-mashing.

## Development

```sh
pnpm test
pnpm build
```

## Deploy online

Total 22 can deploy as a Cloudflare Worker with a room relay:

```sh
pnpm cf:deploy
```

Send the deployed link to friends, make a room, and play.
