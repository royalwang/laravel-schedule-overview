# Monitor Laravel scheduled jobs with ease

This Laravel 5 package allows you to monitor all scheduled jobs, adding this command "php artisan schedule:overview". This command will print all relevant informations about jobs.

## Getting Started

These instructions allows you to install the package into an existing Laravel app.

### Prerequisities

A Laravel 5 installation up & running.

### Installation

You can install this package via Composer using:

```bash
composer require michelecurletta/laravel-schedule-overview
```

You must also install this service provider.

```php
// config/app.php
'providers' => [
    ...
    MicheleCurletta\LaravelScheduleOverview\ScheduleOverviewServiceProvider::class,
    ...
];
```

### Usage

#### Default view

Once you have installed the package, you can run the following command:

```bash
php artisan schedule:overview
```

You will see the list of scheduled jobs with all relevant details.

![Laravel schedule overview](/images/schedule_overview.png?raw=true "Laravel schedule overview")

#### Detailed view

```bash
php artisan schedule:overview --detailed
```

This will display a slightly more detailed view of the scheduled tasks, much like the [Indatus/dispatcher](https://github.com/Indatus/dispatcher)-package for Laravel 4.

![Laravel schedule overview detailed](/images/schedule_overview_detailed.png?raw=true "Laravel schedule overview detailed")

All done!

### Suggestion

Use this command before you deploy you applications, in order to check the jobs frequency and timing.
Enjoy.
