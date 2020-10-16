SolidusUserRoles
=====================

[![CircleCI](https://circleci.com/gh/boomerdigital/solidus_user_roles.svg?style=svg)](https://circleci.com/gh/boomerdigital/solidus_user_roles)


SolidusUserRoles gives an admin the ability to create custom roles for their employees to restrict or allow access to certain sections in the admin panel.

Installation
------------

Add solidus_user_roles to your Gemfile:

```ruby
gem 'solidus_user_roles', github: 'boomerdigital/solidus_user_roles'
```

Bundle your dependencies and run the installation generator:

```shell
bundle
bundle exec rails g solidus_user_roles:install
```

Remember to seed or run:
```shell
rake solidus_user_roles:load_seeds
```

Admin Panel
-----------
An admin is the only user who has the ability to add or remove roles from other users.
![image](https://cloud.githubusercontent.com/assets/6445334/14432566/b90ae0b4-ffd8-11e5-832c-8692dbb437bb.png)
![image](https://cloud.githubusercontent.com/assets/6445334/14432655/0c5c7a84-ffd9-11e5-8463-366fa88b774f.png)
![image](https://cloud.githubusercontent.com/assets/6445334/14432674/22dadc60-ffd9-11e5-97c2-3e9719427140.png)


Testing
-------

First bundle your dependencies, then run `rake`. `rake` will default to building the dummy app if it does not exist, then it will run specs. The dummy app can be regenerated by using `rake test_app`.

```shell
bundle
bundle exec rake
```

When testing your applications integration with this extension you may use it's factories.
Simply add this require statement to your spec_helper:

```ruby
require 'solidus_user_roles/factories'
```

Copyright (c) 2016 [name of extension creator], released under the New BSD License
