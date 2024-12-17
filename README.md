# Dagger PHP SDK

## Installation

### Step 1.1 - php stan test your local source code from the CLI

Assuming your `source` code is locally here, then it will mount the whole path of `.` and then within that it will test the `.` directory within the current directory

``` bash
dagger shell -c 'github.com/dragoonis/dagger-phpstan | phpstan 8.1 . src'
```

## Step 1.2 - phpstan test a remote git repo from the CLI

Assuming you have already run `dagger init` on your local repo, you can reference a remote repository URL instead of a local path, in `--source`

Note the branch name is separated by a `#` character

``` bash
dagger shell -c 'github.com/dragoonis/dagger-phpstan | phpstan 8.1 https://github.com/dragoonis/Sylius\#2.0 src'
```

### Step 2 - phpstan test your source using PHP code

You can install the phpstan module, into your local project's dagger module, and then invoke it from inside the PHP source code

``` bash
dagger install https://daggerverse.dev/mod/github.com/dragoonis/dagger-phpstan@30d7518bdf42c238940790110c6169cbb7d3dcc9
```

Add this code to your local dagger module at `.` dagger/src/<YourModule.php>
