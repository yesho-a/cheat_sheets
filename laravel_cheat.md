# Laravel Cheat Sheet

**1. Make migration**

> `php artisan make:migration create_post_table--table=post`.

The above creates a migration for a database table named post.

**Create Migration to Add Column to Table**

> `php artisan make:migration add_image_to_posts_table --table=posts`

Creates a migration to add column named image to the posts table.

**Delete Column from Table**

_Option 1 : Create a migration to delete column_

> `php artisan make:migration delete_image_from_posts_table --table=posts`

Creates a migration to delete a column named image from the posts table.

_Option 2 : Use down() function in migration.php_

Add the column to be deleted inside the down function as shown below.

> `Schema::table('posts', function (Blueprint $table) { $table->string('image'); });`

Then run the code below

> ` php artisan migrate:rollback`

This will remove the image column from the posts table.

**2. Make Model**

> `php artisan make:model Post`

Creates a model Post
