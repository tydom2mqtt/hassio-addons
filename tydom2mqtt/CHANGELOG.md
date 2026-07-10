# Changelog

Evolutions notables de l'add-on tydom2mqtt.

## 1.1.3

- FIX : l'add-on tournait en utilisateur non-root, ce qui empechait la
  lecture de `/data/options.json` (ecrit en root par le Supervisor) et
  provoquait un crash au demarrage (PermissionError [Errno 13]). L'image
  tourne de nouveau en root.

## 1.1.2

- BREAKING : l'architecture `i386` n'est plus supportee. L'image du fork
  `ghcr.io/skandass/tydom2mqtt` est publiee uniquement pour `armhf` (arm/v6),
  `armv7` (arm/v7), `aarch64` (arm64) et `amd64`. Les installations `i386`
  ne peuvent plus tirer l'image ; migrez vers une plateforme 64 bits ou amd64.

## 1.1.1

- L'add-on utilise desormais l'image du fork `ghcr.io/skandass/tydom2mqtt`
  (au lieu de `ghcr.io/tydom2mqtt/tydom2mqtt`).
- Image multi-architecture : `armhf` (arm/v6), `armv7`, `aarch64`, `amd64`.
- URL de l'add-on et du depot alignees sur le fork skandass.

> Note : le schema de version repart en 1.x pour le fork skandass.
> L'add-on upstream referencait l'image `ghcr.io/tydom2mqtt/tydom2mqtt:3.6.0`.
