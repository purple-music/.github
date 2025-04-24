# Purple Music 💜🎵

### A fullstack SaaS platform for music studio booking

![изображение](https://github.com/user-attachments/assets/7f949b8b-1016-47ff-9aad-c406ab2d7c18)
![image(2)](https://github.com/user-attachments/assets/8d68540e-889d-4c7b-b9df-71a80fb4132e)


https://purple.porkenstein.ru

Welcome to the GitHub organization for Purple Music, a real-world application I’m building to help a friend automate bookings and studio management for their music business. This project has been my main focus since graduating, giving me hands-on experience with fullstack development, system design, and DevOps.

> ⚠️ This project is still a work in progress. It is in production, but might be broken. Some components (tests, Storybook) are currently broken but will be updated.

---

## 🧩 Overview

Purple Music is a modular system composed of:

- **Frontend**: Built with Next.js and React, styled with Tailwind and React Aria.
- **Backend**: Built with NestJS, using Prisma ORM and PostgreSQL.
- **Telegram Mini App**: Smooth Telegram-based auth for quick access.
- **Infrastructure**: Home lab-powered Docker deployment.

## 🖥️ Frontend

- **Framework**: Next.js (originally used NextAuth + Prisma)
- **Data Fetching**: React Query + Axios
- **Authentication**: JWT stored in HTTP-only cookies; integrates with multiple auth providers
- **UI**: Custom components using Tailwind + React Aria
- **Screens**: Dashboard, Calendar, Booking (all designed by me in Figma)
- **Types**: Uses OpenAPI generated types to keep it TS-friendly!
- **Features**:
  - Email verification & password reset via tokens
  - Telegram WebApp integration for auth
  - (Broken) Storybook setup

## 🧠 Backend

- **Framework**: NestJS
- **ORM**: Prisma + PostgreSQL (schema designed from scratch)
- **Auth**: Passport.js (supports credentials, Telegram, Yandex)
- **Emails**: Resend integration for transactional emails
- **Docs**: Swagger & OpenAPI for API exploration
- **Tests**: Some initial tests exist (currently broken)

## 🤖 Telegram Mini App

- Implements Telegram WebApp API for embedded auth experience
- Integrated with frontend for seamless login via Telegram

## 🏗️ Infrastructure

- **Dockerized microservices**: Each component is containerized and stored in the GitHub registry
- **Deployment**: Managed via docker-compose in a dedicated [infra repo](https://github.com/purple-music/infra)
- **Home Lab**: Built and configured my own home server to host and manage the stack

## 🚧 What I'm working on next

- Fixing tests and Storybook
- Improving auth UX across platforms
- Adding Google Calendar integration
- Preferrably to scale to meta-app with being able to manage multiple booking organizations!
