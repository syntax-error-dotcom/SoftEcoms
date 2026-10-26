para mo dagan ang database
Pag himog database na name softecoms

tapos i import tong sql na akong gi hatag tenkies


# Sweetclaire (SoftEcoms)

## Requirements
- XAMPP (Apache + MySQL + PHP)
- Node.js
- Git
- Tested with: Node vX.X, PHP X.X   <!-- fill in: node --version, php --version -->

## How to run

1. Clone into XAMPP's htdocs. The folder name must stay `SoftEcoms`:
   ```bash
   cd C:\xampp\htdocs
   git clone https://github.com/syntax-error-dotcom/SoftEcoms.git
   cd SoftEcoms
   ```

2. Install the Node packages:
   ```bash
   npm ci
   ```

3. Set up the environment file:
   - Copy `env template.txt` and rename the copy to `.env`
   - Fill in the missing values only. Leave the pre-filled ones as they are.

4. Set up the database:
   - Start Apache and MySQL in XAMPP
   - Open phpMyAdmin, create a database, and import `softecoms.sql`
   - Make sure the database name in `.env` matches

5. Start the Node server (handles login and register):
   ```bash
   node server.js
   ```

6. Open http://localhost/SoftEcoms/public/

## Notes
- Product images are in `public/assets/product_img/` (resized to keep the repo small).
- Never commit `.env`. It's in `.gitignore`.
