# Restaurant App: Client

React front end for a restaurant discovery and table-booking platform. It has three portals in one app: a **customer** site, a **partner** (restaurant owner) dashboard and an **admin** console. Pairs with [restaurant-app-server](https://github.com/cyber-traveller/restaurant-app-server).

![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=white)
![Chakra UI](https://img.shields.io/badge/Chakra_UI-319795?logo=chakraui&logoColor=white)
![Mapbox](https://img.shields.io/badge/Mapbox-000000?logo=mapbox&logoColor=white)

## Features

**Customers:** register and log in, browse restaurants and cuisines, view restaurant details and reviews, book tables, manage bookings and profile, reset forgotten passwords.

**Partners (`/partner/*`):** manage restaurant details and menus, dashboard, view orders.

**Admins (`/admin/*`):** dashboard, user and partner management, approve pending restaurants, manage cuisines and menu categories.

Maps and directions use Mapbox. Payments use Razorpay. Firebase is used for Google and phone sign-in and for file storage.

## Tech stack

React (Create React App), Chakra UI, Material UI, Font Awesome, Mapbox GL, Firebase, Razorpay.

## Getting started

```bash
git clone https://github.com/cyber-traveller/restaurant-app-client.git
cd restaurant-app-client
npm install
```

Create a `.env` file:

| Variable | Purpose |
| --- | --- |
| `REACT_APP_SERVERURL` | URL of restaurant-app-server |
| `REACT_APP_MAPBOXTOKEN` | Mapbox access token |
| `REACT_APP_RAZORPAYKEY` | Razorpay key id |
| `REACT_APP_APIKEY`, `REACT_APP_AUTHDOMAIN`, `REACT_APP_PROJECTID`, `REACT_APP_STORAGEBUCKET`, `REACT_APP_MESSAGINGSENDERID`, `REACT_APP_APPID` | Firebase web config |

```bash
npm start
```

| Command | What it does |
| --- | --- |
| `npm start` | Dev server |
| `npm run build` | Production build |
| `npm test` | Test runner |
