# Laravel Cheat Sheet

**Make migration**

> `php artisan make:migration create_post_table--table=post`.

The above creates a migration for a database table named post.

**Create Migration to Add Column to Table**

> `php artisan make:migration add_image_to_posts_table --table=posts`

Creates a migration to add column named image to the posts table.

**Create Migration to Delete Column from Table**

> `php artisan make:migration delete_image_from_posts_table --table=posts`

Creates a migration to delete a column named image from the posts table.

**Make Model**
