# Filmpedia

A movie and web-series catalogue built in PHP and MySQL, with a public-facing site and a separate admin panel for managing the library.

## What it does

- **Public catalogue** — browse movies and web series by genre, search titles, and open a detail page for each one
- **Admin panel** (`Admin/`) — dashboard with counts and charts, add/edit movie and series entries, manage genres, upload poster images, and log out
- **Genres** — create, edit and delete genres and attach them to titles

## Structure

```
Admin/                 admin panel (auth, CRUD pages, dashboard, template assets)
Admin/movies_img/      uploaded poster artwork
Admin/config.php       database connection used by the admin pages
```

## Requirements

- PHP 7+ with `mysqli`
- MySQL or MariaDB
- Apache (XAMPP/WAMP/Laragon)

## Setup

1. Import the database schema into MySQL.
2. Set the connection credentials in `Admin/config.php`.
3. Serve the folder from your web root; the catalogue loads from the root, the admin panel from `/Admin/index.php`.

## Notes

Early full-stack PHP project. Poster images and third-party front-end libraries (Owl Carousel, Bootstrap, Chart.js, tempusdominus) are committed in the repo, which is why the tree is on the large side.
