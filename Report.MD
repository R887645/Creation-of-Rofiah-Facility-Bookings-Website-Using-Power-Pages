# Rofiah Facility Bookings Website — Power Pages + Dataverse

A no-code facility booking website built entirely with Microsoft Power Pages and Dataverse. Clients can browse and book available spaces, including conference rooms, event halls, office spaces, and sports facilities — through a clean, professional web portal. A built-in issue submission form allows clients to report facility problems directly from their user dashboard.

---

## Features

- Clients can browse and book four facility types: conference rooms, event halls, office spaces, and sports facilities
- User dashboard where clients manage their bookings
- Built-in issue/rectification form for clients to report facility problems directly from their dashboard
- All booking and issue data stored and managed in Microsoft Dataverse
- Secure, role-based access for clients via Power Pages authentication

---

## Architecture

- **Frontend:** Microsoft Power Pages (public-facing booking website)
- **Backend/Database:** Microsoft Dataverse (stores bookings, facility data, and issue submissions)
- **User Dashboard:** Power Pages authenticated portal with embedded issue submission form

---

## 🏗️ Facilities Available for Booking

| Facility | Description |
|---|---|
| Conference Rooms | Professional meeting spaces for teams and clients |
| Event Halls | Large spaces for corporate events and gatherings |
| Office Spaces | Flexible workspaces for individuals and teams |
| Sports Facilities | Courts and activity spaces for recreational use |

---

## 🖥️ Part 1 — Website & Data Model Setup

I started by designing the data model in **Microsoft Dataverse** using Copilot Studio, creating tables to store all the information the portal would need. The core tables include:

`Facility` · `Booking` · `Client` · `Facility Type` · `Availability` · `Issue Report`

Each facility record holds details like name, type, capacity, and availability status. The Booking table links a client to a specific facility with a date and time slot. The Issue Report table captures client-submitted problems, including a description, the affected facility, and submission date.

With the data model in place, I set up the **Power Pages site**, configured the site's pages, and connected it to the Dataverse environment. I applied custom branding — logo, colour scheme, and layout — to give the portal a professional look consistent with the Rofiah Facility identity.

---
![My Image](https://github.com/R887645/Creation-of-Rofiah-Facility-Bookings-Website-Using-Power-Pages/blob/main/Power%20Pages_1.png?raw=true)

## ⚙️ Part 2 — Booking Flow & User Dashboard

The public-facing side of the website allows visitors to view available facilities, check availability, and submit a booking request. Each booking is written directly to the Dataverse **Booking** table on submission.

For authenticated clients, I built a **User Dashboard** accessible after login. From the dashboard, clients can view their current and past bookings at a glance. I also created a dedicated **Issue Submission Form** embedded directly on the dashboard page, allowing clients to flag any facility problems — such as maintenance issues or equipment faults — without leaving the portal. Submitted issues are stored in the **Issue Report** table in Dataverse for the facilities team to review and action.

Access to the dashboard is protected by Power Pages' built-in authentication, ensuring only registered clients can view their data and submit issues.

![My Image](https://github.com/R887645/Creation-of-Rofiah-Facility-Bookings-Website-Using-Power-Pages/blob/main/power%20page%202.png?raw=true)

![My Image](https://github.com/R887645/Creation-of-Rofiah-Facility-Bookings-Website-Using-Power-Pages/blob/main/power%20page%202.png?raw=true)

[Watch the snapshot Video of the website](https://drive.google.com/file/d/1XmmaANCHwK_EyUodV7Zs0HKfWExk6Nmn/view?usp=sharing)

---

## 📋 Dataverse Tables

| Table | Purpose |
|---|---|
| Facility | Stores all facility records and details |
| Facility Type | Categorises facilities (conference, event, office, sports) |
| Availability | Tracks available time slots per facility |
| Booking | Records all client bookings |
| Client | Stores registered client profiles |
| Issue Report | Logs client-submitted facility issues |

---

## 📸 Screenshots

| View | File |
|---|---|
| Homepage / Facility listing | `homepage.png` |
| Booking form | `booking-form.png` |
| User dashboard | `dashboard.png` |
| Issue submission form | `issue-form.png` |
| Dataverse tables | `dataverse.png` |

---

## 💡 Built With

- Microsoft Power Pages
- Microsoft Dataverse
- Copilot Studio

---

## 👩🏽‍💻 Author

**Rofiah Abdul-Azeez**
Power Platform Developer · Creator of Rofiah Techie Hub

---

*Crafted with ❤️ by Rofiah Techie Hub*
