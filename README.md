# pass.in 🎟️

**pass.in** is an application for **managing participants in in-person events**.

The platform allows event organizers to create events and open a public registration page.

Registered participants can generate a badge (credential) to check in on the event day.

The system scans the participant’s badge (via QR code) to authorize entry into the event.

---

## ✅ Requirements

### Functional Requirements

- [x] Organizers must be able to register a new event.
- [x] Organizers must be able to view event details.
- [x] Organizers must be able to view a list of participants.
- [x] Participants must be able to register for an event.
- [x] Participants must be able to view their registration badge.
- [x] Participants must be able to check in at the event.

### Business Rules

- [x] A participant can only register for an event once.
- [x] A participant can only register for events with available spots.
- [x] A participant can only check in to an event once.

### Non-Functional Requirements

- [x] Event check-in is performed through a QR Code.

---

## 🚀 How to Run the Project

### Seed the database

```bash
npx prisma seed
```

### Run in production mode
```bash
npm run build
npm start
```

### Run database migrations
```bash
npm run db:migrate
```
