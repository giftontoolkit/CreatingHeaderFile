# Creating Heading files and Call in Index.php

- We will use multiple headers, therefore we move all headers in one folder `header`. And the we used `get_template_part()`.
- If there is only one header file then there is no need to separate folder. In this case, we will create `header.php` in root directory and use `get_header()`.

## Version 1 (v1)

- Create landing-header.php in `v1/header` folder
- The `landing-header.php` contains `<header>` tag and `landing-header` CSS-class. On base of these two things, we will further style it in `functions.php`.
- Code for landing-header.php is given below

```ruby
<header class="landing-header">
    <div class="container" style="border: 1px solid red">
        <h1>Welcome to our theme</h1>
        <p>Empowering your eCommerce journey with customization.</p>
    </div>
</header>
```

- The `index.php` file will call `landing-header.php` file by using follwoing line.

```ruby
<?php get_template_part('header/landing-header'); ?>
```
