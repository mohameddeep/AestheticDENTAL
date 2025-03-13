
## Requirements

- Local server, e.g., XAMPP, WAMP, Laragon (Laragon is preferred).

- PHP 8.1 (Required for Laravel 10).

## Installation

- Clone the project:

```bash
  git clone https://github.com/elryad-web/initial-backend-project.git
```

- Install composer packages:

```bash
  composer install
```

- Setup your environment:

Rename `.env.example` file to `.env`, then generate your Laravel app key.

```bash
  php artisan key:generate
```

- Generate new JWT secret key:

```bash
  php artisan jwt:secret
```

- Migrate and seed database:

```bash
  php artisan migrate --seed
```

- Link your storage folder with public folder:

```bash
  php artisan storage:link
```

- Clear cache:

```bash
  php artisan optimize:clear
```

## Documentation
This system is designed to manage various aspects of a dental clinic, featuring four distinct user roles:

Admin: Oversees the entire system, managing users and settings.

Patient: Accesses personal medical records and schedules appointments.

Services: doctor introduce many service and patient will book one of them
Appointment Management: Facilitates scheduling and tracking of patient appointments.
Patient Records: Allows creation of PDF reports detailing general medical information and specific reservation details.
