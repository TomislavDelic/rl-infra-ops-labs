# SSH hardening (key-only)

Cilj: siguran SSH pristup na Ubuntu VM (login samo SSH ključem, bez lozinke; root login zabranjen).

## Što je napravljeno
- Generiran ED25519 ključ na Windowsu
- Public key dodan u `~/.ssh/authorized_keys`
- Password login ugašen (`PasswordAuthentication no`, `KbdInteractiveAuthentication no`)
- Verifikacija: FAIL bez ključa, OK s ključem (`sshd -T`)

## Artefakti
- PDF report u ovom folderu
