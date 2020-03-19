# Advanced Streaming Tech

## 1

- Review

## 2

- Unit & Feature Testing
  - Unit and Feature Tests
    - Unit test tests specific code
    - Feature test tests entire feature
      - Feature tests "do not" test logic
  - Created testing in scripts
  - Laravel uses PHPunit to test
  - Tests require assertions
    - Checks to be used by the tester
    - Tests can have many assertions
  - Create a test `php artisan make:test SomeTest`
    - Can be passed flag `-unit` to create a unit test
  - All methods must be prefixed with `test`
  - Run specific test: `phpunit tests/[testtype]/SomeTest.php`
  - phpunit.xml contains test data
  - ASSERTIONS
    - True, False, Equals, Null, Contains, Count, Empty
  - Good unit tests:
    - Test one thing
    - Verify only things about the thing
    - Doesn't depend on external data
      - Create data with the test
    - Doesn't depend on external resources
      - Create resources with the test
    - Should be able to run tests in parallel

## 3

- Browser Testing
  - Uses Laravel Dusk:
  - `composer require --dev laravel/dusk`
  - `php artisan dusk:install`
  - Running Dusk: `php artisan dusk`
  - Make test: `php artisan dusk:make LoginTest`
  - Dusk Selectors: blade template elements to bind selection to
    - IE: `dusk="login-button"`

## 4

- Vue & Laravel

## 5

- Vue & Laravel p2
  - Built a transformer
