# Dagger PHP SDK

## Installation

Step 1 - install this module on your existing project

``` bash
dagger install https://daggerverse.dev/mod/github.com/dragoonis/dagger-phpstan@30d7518bdf42c238940790110c6169cbb7d3dcc9
```

Step 2.1 - execute this from the command line, mounting your app's source code

Assuming your source code is locally here, then it will mount the whole path of `.` and then within that it will test the `.` directory within the current directory

``` bash
dagger call phpstan --php-version=8.3 --source=. --path-to-test=src
```

Step 2.2 - execute this from the command line, cloning down a repo git repository

Assuming your source code is locally here, then it will mount the whole path of `.` and then within that it will test the `.` directory within the current directory

``` bash
dagger call phpstan --php-version=8.3 --source=https://github.com/dragoonis/Sylius#2.0 --path-to-test=src
```
