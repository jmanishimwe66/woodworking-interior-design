# Woodworking & Interior Design

A portfolio and business website for a woodworking and interior design professional. The platform showcases completed projects, presents services, and helps customers request custom commissions or inquire about available products.

## Project Objectives

- Showcase craftsmanship and completed projects.
- Present services and custom design capabilities.
- Generate commission and quotation requests.
- Provide a simple catalogue for selected ready-made products.

## Key Features

- Homepage introducing the business.
- Portfolio and project gallery.
- Services for woodworking, furniture, and interior design.
- About the designer or studio.
- Custom commission and quotation inquiry form.
- Simple product catalogue or shop.
- Contact information and social links.
- Product ordering flow if required.

## Technology Stack

- **Frontend:** React.js, TypeScript
- **Backend:** Python, FastAPI
- **Database:** Supabase PostgreSQL
- **Storage:** Supabase Storage for project images, if required
- **Authentication:** Supabase Auth for protected management features, if required
- **Containerization:** Docker and Docker Compose

## Architecture

The React frontend presents the portfolio, services, and products. FastAPI handles custom backend operations, such as commission inquiries or order workflows, when needed. Supabase supports persistent data and file storage. Docker provides a consistent development environment.

## Getting Started

### Prerequisites

- Node.js and npm
- Python 3
- Docker and Docker Compose
- A Supabase project

### Environment Configuration

Create local environment files based on `.env.example`.

Frontend variables:

- `VITE_SUPABASE_URL`
- `VITE_SUPABASE_ANON_KEY`

Backend variables, where required:

- `SUPABASE_URL`
- `SUPABASE_SERVICE_ROLE_KEY` — server-side only, if elevated access is needed.

Never commit production credentials or expose privileged keys in frontend code.

### Development

Install frontend dependencies:

```bash
cd frontend
npm install
npm run dev
```

Install backend dependencies according to the project's Python configuration and start FastAPI using the configured application entry point.

Once Docker configuration is in place, start the application with:

```bash
docker compose up --build
```

## Initial Scope

The first release focuses on portfolio presentation, service information, commission inquiries, and a simple product catalogue if required. Advanced product customization, 3D previews, automated quotations, and complex e-commerce are excluded unless separately approved.

## Quality Assurance

Test portfolio navigation, image responsiveness, inquiry forms, validation, and mobile layouts.

## Project Status

In development.

## License

To be determined by the project owner.
