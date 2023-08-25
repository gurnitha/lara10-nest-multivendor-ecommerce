# lara10-nest-multivendor-ecommerce
Training membuat aplikasi multivendor ecommerce menggunakan Laravel versi 10
Github: https://github.com/gurnitha/lara10-nest-multivendor-ecommerce


## 1. PROJECT

#### 1.1 Create project with breeze

        new file:   .editorconfig
        new file:   .env.example
        new file:   .gitattributes
        modified:   README.md
        new file:   app/Console/Kernel.php
        new file:   app/Exceptions/Handler.php
        new file:   app/Http/Controllers/Auth/AuthenticatedSessionController.php
        new file:   app/Http/Controllers/Auth/ConfirmablePasswordController.php
        new file:   app/Http/Controllers/Auth/EmailVerificationNotificationController.php
        new file:   app/Http/Controllers/Auth/EmailVerificationPromptController.php
        new file:   app/Http/Controllers/Auth/NewPasswordController.php
        new file:   app/Http/Controllers/Auth/PasswordController.php
        new file:   app/Http/Controllers/Auth/PasswordResetLinkController.php
        new file:   app/Http/Controllers/Auth/RegisteredUserController.php
        new file:   app/Http/Controllers/Auth/VerifyEmailController.php
        new file:   app/Http/Controllers/Controller.php
        new file:   app/Http/Controllers/ProfileController.php
        new file:   app/Http/Kernel.php
        new file:   app/Http/Middleware/Authenticate.php
        new file:   app/Http/Middleware/EncryptCookies.php
        new file:   app/Http/Middleware/PreventRequestsDuringMaintenance.php
        new file:   app/Http/Middleware/RedirectIfAuthenticated.php
        new file:   app/Http/Middleware/TrimStrings.php
        new file:   app/Http/Middleware/TrustHosts.php
        new file:   app/Http/Middleware/TrustProxies.php
        new file:   app/Http/Middleware/ValidateSignature.php
        new file:   app/Http/Middleware/VerifyCsrfToken.php
        new file:   app/Http/Requests/Auth/LoginRequest.php
        new file:   app/Http/Requests/ProfileUpdateRequest.php
        new file:   app/Models/User.php
        new file:   app/Providers/AppServiceProvider.php
        new file:   app/Providers/AuthServiceProvider.php
        new file:   app/Providers/BroadcastServiceProvider.php
        new file:   app/Providers/EventServiceProvider.php
        new file:   app/Providers/RouteServiceProvider.php
        new file:   app/View/Components/AppLayout.php
        new file:   app/View/Components/GuestLayout.php
        new file:   artisan
        new file:   bootstrap/app.php
        new file:   bootstrap/cache/.gitignore
        new file:   composer.json
        new file:   composer.lock
        new file:   config/app.php
        new file:   config/auth.php
        new file:   config/broadcasting.php
        new file:   config/cache.php
        new file:   config/cors.php
        new file:   config/database.php
        new file:   config/filesystems.php
        new file:   config/hashing.php
        new file:   config/logging.php
        new file:   config/mail.php
        new file:   config/queue.php
        new file:   config/sanctum.php
        new file:   config/services.php
        new file:   config/session.php
        new file:   config/view.php
        new file:   database/.gitignore
        new file:   database/factories/UserFactory.php
        new file:   database/migrations/2014_10_12_000000_create_users_table.php
        new file:   database/migrations/2014_10_12_100000_create_password_reset_tokens_table.php
        new file:   database/migrations/2019_08_19_000000_create_failed_jobs_table.php
        new file:   database/migrations/2019_12_14_000001_create_personal_access_tokens_table.php
        new file:   database/seeders/DatabaseSeeder.php
        new file:   package-lock.json
        new file:   package.json
        new file:   phpunit.xml
        new file:   postcss.config.js
        new file:   public/.htaccess
        new file:   public/build/assets/app-7a4a8d6c.css
        new file:   public/build/assets/app-cd8a593d.js
        new file:   public/build/manifest.json
        new file:   public/favicon.ico
        new file:   public/index.php
        new file:   public/robots.txt
        new file:   resources/css/app.css
        new file:   resources/js/app.js
        new file:   resources/js/bootstrap.js
        new file:   resources/views/auth/confirm-password.blade.php
        new file:   resources/views/auth/forgot-password.blade.php
        new file:   resources/views/auth/login.blade.php
        new file:   resources/views/auth/register.blade.php
        new file:   resources/views/auth/reset-password.blade.php
        new file:   resources/views/auth/verify-email.blade.php
        new file:   resources/views/components/application-logo.blade.php
        new file:   resources/views/components/auth-session-status.blade.php
        new file:   resources/views/components/danger-button.blade.php
        new file:   resources/views/components/dropdown-link.blade.php
        new file:   resources/views/components/dropdown.blade.php
        new file:   resources/views/components/input-error.blade.php
        new file:   resources/views/components/input-label.blade.php
        new file:   resources/views/components/modal.blade.php
        new file:   resources/views/components/nav-link.blade.php
        new file:   resources/views/components/primary-button.blade.php
        new file:   resources/views/components/responsive-nav-link.blade.php
        new file:   resources/views/components/secondary-button.blade.php
        new file:   resources/views/components/text-input.blade.php
        new file:   resources/views/dashboard.blade.php
        new file:   resources/views/layouts/app.blade.php
        new file:   resources/views/layouts/guest.blade.php
        new file:   resources/views/layouts/navigation.blade.php
        new file:   resources/views/profile/edit.blade.php
        new file:   resources/views/profile/partials/delete-user-form.blade.php
        new file:   resources/views/profile/partials/update-password-form.blade.php
        new file:   resources/views/profile/partials/update-profile-information-form.blade.php
        new file:   resources/views/welcome.blade.php
        new file:   routes/api.php
        new file:   routes/auth.php
        new file:   routes/channels.php
        new file:   routes/console.php
        new file:   routes/web.php
        new file:   storage/app/.gitignore
        new file:   storage/app/public/.gitignore
        new file:   storage/framework/.gitignore
        new file:   storage/framework/cache/.gitignore
        new file:   storage/framework/cache/data/.gitignore
        new file:   storage/framework/sessions/.gitignore
        new file:   storage/framework/testing/.gitignore
        new file:   storage/framework/views/.gitignore
        new file:   storage/logs/.gitignore
        new file:   tailwind.config.js
        new file:   tests/CreatesApplication.php
        new file:   tests/Feature/Auth/AuthenticationTest.php
        new file:   tests/Feature/Auth/EmailVerificationTest.php
        new file:   tests/Feature/Auth/PasswordConfirmationTest.php
        new file:   tests/Feature/Auth/PasswordResetTest.php
        new file:   tests/Feature/Auth/PasswordUpdateTest.php
        new file:   tests/Feature/Auth/RegistrationTest.php
        new file:   tests/Feature/ExampleTest.php
        new file:   tests/Feature/ProfileTest.php
        new file:   tests/TestCase.php
        new file:   tests/Unit/ExampleTest.php
        new file:   vite.config.js

#### 1.2 Create and connect with db

        mysql> CREATE DATABASE lara10_nest_multivendor_ecommerce;
        Query OK, 1 row affected (0.09 sec)

#### 1.3 Run migration to create tables and register a new user

        mysql> SELECT id, name, email FROM users;                                        
        +----+------------+---------------------+                                        
        | id | name       | email               |                                        
        +----+------------+---------------------+                                        
        |  1 | superadmin | superadmin@mail.com |                                        
        +----+------------+---------------------+                                        
        1 row in set (0.00 sec)    

