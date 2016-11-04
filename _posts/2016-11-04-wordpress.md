---
layout: page
title: "WordPress"
category: examples
date: 2016-11-04 15:00:07
---

# How to create WordPress site with gdev

In this example we will create new WordPress site named **mysite.com**.

## Installation
```bash
# Create new project in your Projects folder
$ git clone https://github.com/devgeniem/wp-project ~/Projects/mysite

$ cd ~/Projects/mysite

# Install composer packages
$ composer install --ignore-platform-reqs

# Change default addresses from the project wordpress.test -> mysite.test
$ sed -i 's|wordpress.test|mysite.test/g' docker-compose.yml

# Change your own name and details into composer.json authors block
$ edit composer.json

# Startup development of the site
$ gdev up
```

## Next steps
Choose what theme framework you want to use and clone it into `web/app/themes/my-theme-name`.
