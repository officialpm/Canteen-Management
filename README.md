# Canteen Management System (PHP)

A simple **PHP + MySQL** web app for canteen-style ordering and administration.

From the repo structure, this project includes separate areas for admin/user login and pages for orders, feedback, notifications, and profiles.

## Tech stack

- PHP
- MySQL (PDO)
- HTML/CSS/JS (includes Bootstrap assets in the repo)

## Local setup (basic)

> Note: a database schema dump is **not included** in this repository, so you’ll need to create the tables yourself (or recover them from an older environment).

1. Start a local MySQL instance.
2. Create a database called `cms`.
3. Update credentials in:

- `includes/config.php`

```php
define('DB_HOST','localhost');
define('DB_USER','root');
define('DB_PASS','root');
define('DB_NAME','cms');
```

4. Serve the project with your local PHP server:

```bash
php -S localhost:8000
```

5. Visit `http://localhost:8000/`.

## Repo structure

- `includes/` — shared config + layout includes
- `admin/`, `adminlogin/` — admin UI
- `userlogin/` — user auth UI
- `docs/` — static docs/pages assets

## Notes

This is a learning/portfolio project. If you intend to deploy it, review security (auth, SQL injection protection, password storage, etc.).

## License

No license specified.
