# Real-Time Dispatch System 🚗

A full-stack, real-time logistics and dispatch platform modeling real-world workflows (Client, Driver, Dispatcher) using WebSockets, state machine logic, and interactive spatial mapping.

## 🏗️ System Architecture & Scope

1. **Client Interface:** Request rides, set pickup/drop-off coordinates, specify accessibility requirements, and track driver arrival.
2. **Driver View (Mobile Web/PWA):** Receive ride requests, accept/reject assignments, and push real-time status updates using a strict state machine (`Assigned` -> `En Route` -> `Arrived` -> `Completed`).
3. **Dispatcher Dashboard:** Monitor all active drivers, current ride statuses, and system metrics on a live Mapbox interface via persistent WebSockets.

## 🛠️ Tech Stack

* **Frontend:** React, TailwindCSS, Mapbox GL JS
* **Backend:** Node.js (Express), Socket.io
* **Database:** PostgreSQL / Supabase (PostGIS for spatial queries)
* **Testing:** Jest, Cypress / Playwright

## 🚀 Getting Started

### Prerequisites
* Node.js (v18+)
* npm or yarn
* PostgreSQL / Supabase account
* Mapbox API Token

### Installation
1. Clone the repository:
```bash
git clone https://github.com/LuthandoNgombane/dispatch-app-setup.git
cd dispatch-app-setup
```

2. Install dependencies for server and client:
```bash
cd server && npm install
cd ../client && npm install
```


3. Set up environment variables (`.env`):
```env
PORT=5000
DATABASE_URL=your_postgres_url
MAPBOX_ACCESS_TOKEN=your_mapbox_token

```


4. Run the development server:
```bash
# In /server
npm run dev
# In /client
npm run dev

```



## 🤝 Contributing & Issue Board

We welcome contributions! Check out the [Issues tab](https://github.com/LuthandoNgombane/dispatch-app-setup/issues) to find open tasks categorized by layer (`frontend`, `backend`, `database`, `good first issue`). Comment on an issue to get assigned.
