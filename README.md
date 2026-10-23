# Cash Out

A money-themed wave-survival shooter in the style of Black Ops Zombies, with a
PS1 horror look. It runs in the browser and needs no install or build step.
It works with keyboard and mouse, or with touch controls on phones and
tablets (play in landscape).

- Fight off rounds of the bank's undead staff: **Salesmen**, **Tax Auditors**
  (fast, from round 4), **Debt Collectors** (throw invoices from range, from
  round 6) and the **Bank President** (tanky boss, every 5th round). Every
  7th round is an **Audit Round**: a swarm of fast Tax Auditors in red fog,
  with a Max Ammo for surviving it. Hits and kills earn cash, and quick kills
  in a row build a cash combo.
- Guns shoot money: Penny Pistol (coins), Bill Blaster (banknotes), Gold Bar
  Shotgun, Market Maker AR, plus the Coin Minigun, Diamond Rifle and Piggy
  Launcher from the **Slot Machine** ($950).
- Spend cash on gun vending machines, the doors to the Trading Floor, Vault
  and Boardroom, perk machines, the **Paper Shredder** trap in the Trading Floor
  doorway and the **Gold Plater** in the Vault, which upgrades a gun to 24K.
- Perks: Health Insurance (more health), Fast Cash (faster reload), Compound
  Interest (+50% cash), Day Trader (faster fire rate), Diversified Portfolio
  (carry a third gun) and Golden Parachute (get back up once).
- Throw Money Bag grenades. Killed enemies sometimes drop Max Ammo, Double
  Cash, Insta-Kill, Market Crash, Bailout (+$1000) or Fire Sale ($10 Slot
  Machine spins).
- Three golden piggy banks are hidden around the bank. Shoot them all for a
  jackpot.
- **Settings** (from the menu or pause screen): picture quality, retro
  effects, field of view, sensitivity and volume. They and your best run are
  saved in the browser.

## Controls

| | Keyboard and mouse | Touch |
|---|---|---|
| Move | WASD, Shift to sprint | Drag on the left side, push all the way up to sprint |
| Look | Mouse or arrow keys | Drag on the right side (or arrow keys on a keyboard) |
| Shoot / aim | Left / right mouse button, or X (or Enter) / C (or right Shift) | FIRE / AIM |
| Jump | Space | JUMP |
| Reload | R | RLD |
| Switch gun | 1, 2, 3, Q or mouse wheel | SWAP |
| Grenade | G | BAG |
| Buy / use | E | USE (shows up next to things you can buy) |
| Pause | Esc or P (Enter starts and resumes) | II |

## Run it

Browsers don't load JS modules from `file://`, so serve the folder with any
static server and open it:

```sh
npx http-server -p 8080 -c-1
# then open http://localhost:8080/
```

It can also be hosted as-is on GitHub Pages (Settings → Pages → deploy from
the `main` branch).

## Credits

Built with plain JS modules and [Three.js](https://threejs.org) r160
(vendored in `vendor/`, MIT), with a PS1-style low-res filter. Graphics and
sounds are generated in code. The only asset file is the pixel font VT323 in
`vendor/fonts/` (SIL Open Font License).
