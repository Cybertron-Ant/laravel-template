# Laravel React Starter Kit

[![Latest Stable Version](https://poser.pugx.org/laravel/react-starter-kit/v/stable)](https://packagist.org/packages/laravel/react-starter-kit) [![Total Downloads](https://poser.pugx.org/laravel/react-starter-kit/downloads)](https://packagist.org/packages/laravel/react-starter-kit) [![License](https://poser.pugx.org/laravel/react-starter-kit/license)](https://packagist.org/packages/laravel/react-starter-kit)

The skeleton application for the Laravel framework, pre-configured with React, Inertia.js, Vite, and Tailwind CSS.

## Requirements

-   PHP >= 8.2
-   Node.js & npm (or yarn/pnpm)
-   Composer

## Installation

1.  **Clone the repository:**
   ```bash
   git clone https://github.com/cybertron-ant/laravel-template.git
   cd your-project-name
   ```

2.  **Install PHP dependencies:**
   ```bash
   composer install
   ```

3.  **Install Node.js dependencies:**
   ```bash
   npm install
   ```
   *or*
   ```bash
   yarn install
   ```
   *or*
   ```bash
   pnpm install
   ```

4.  **Set up your environment file:**
   Copy the example environment file and configure it for your local environment.
   ```bash
   cp .env.example .env
   ```
   Update the database credentials and other settings in the `.env` file.

5.  **Generate an application key:**
   ```bash
   php artisan key:generate
   ```

6.  **Run database migrations:**
   (Ensure your database is created and configured in `.env`)
   ```bash
   php artisan migrate
   ```

7.  **Build frontend assets:**
   ```bash
   npm run build
   ```

## Running the Development Server

To run the development server which includes the PHP server, queue worker, log watcher, and Vite HMR server:

```bash
composer run dev
```

This will typically make the application available at `http://localhost:8000`.

If you need Server-Side Rendering (SSR):

```bash
composer run dev:ssr
```

## Running Tests

To run the PHPUnit test suite:

```bash
php artisan test
```

## Linting and Formatting

-   **Check code formatting (PHP):**
   ```bash
   composer run laravel/pint -- --test
   ```
-   **Apply code formatting (PHP):**
   ```bash
   composer run laravel/pint
   ```
-   **Check code formatting (JS/TS/React):**
   ```bash
   npm run format:check
   ```
-   **Apply code formatting (JS/TS/React):**
   ```bash
   npm run format
   ```
-   **Run ESLint:**
   ```bash
   npm run lint
   ```
-   **Run TypeScript type checking:**
   ```bash
   npm run types
   ```

## Key Technologies

-   [Laravel](https://laravel.com/)
-   [React](https://reactjs.org/)
-   [Inertia.js](https://inertiajs.com/)
-   [Vite](https://vitejs.dev/)
-   [Tailwind CSS](https://tailwindcss.com/)
-   [Ziggy](https://github.com/tighten/ziggy) (for using Laravel routes in JavaScript)
-   [Shadcn UI](https://ui.shadcn.com/) (via components.json and Radix UI dependencies)

## License

This project is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
