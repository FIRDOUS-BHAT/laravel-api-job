# Laravel API with Job Queue, Database, and Event Handling

## Setup

1. Clone the repository
2. Run `composer install`
3. Copy `.env.example` to `.env` and configure your environment variables
4. Run `php artisan key:generate`
5. Run `php artisan migrate`
6. Start the local development server: `php artisan serve`

## Testing the API

1. Run the test suite: `php artisan test`
2. Make a `POST` request to `/api/submit` with JSON payload:
    ```json
    {
        "name": "John Doe",
        "email": "john.doe@example.com",
        "message": "This is a test message."
    }
    ```

## Running the Queue Worker

Start the queue worker to process jobs:

```bash
php artisan queue:work
```
