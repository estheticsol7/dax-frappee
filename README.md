# Dax Frappe

White-labeled Frappe Framework installation.

## Installation

1. Clone this repository:
```bash
git clone https://github.com/estheticsol7/dax-frappee.git
cd dax-frappee
```

2. Install Frappe app:
```bash
bench get-app frappe https://github.com/frappe/frappe
```

3. Install dependencies:
```bash
cd apps/frappe
yarn install
cd ../..
```

4. Create a new site:
```bash
bench new-site mysite.local --admin-password admin --mariadb-root-password root
```

5. Build assets:
```bash
bench build
```

6. Start the server:
```bash
bench start
```

Access at: http://localhost:8001

## Configuration

Edit `sites/common_site_config.json` for site configuration.

## Updating

```bash
git pull origin main
bench update --reset
bench build
```
