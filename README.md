# Scalable E-commerce API!

Using this API you can basically fit any kind of product to sell, that's how it's designed to work.
<br/>

## Features

* Powered by Prisma ORM
* Async operations
* Clean code

## Overview

Routes under _core_ directory handle the primary features:
<br/>
* [Authentication](https://github.com/TheOfficialLOE/NebulaShop#authentication)
* [Finding products](core/routes/main.js)
* [Comment on products](core/routes/comments.js)
* [Vote comments( Like & Dislike )](core/routes/vote.js)
* [Add products to cart](core/routes/cart.js)
* [Purchase products](core/routes/purchases.js)

Routes under _cms_ directory handle Admin Panel operations( only admins and super admins have access to this part ):
<br/>
* [Add new brand](cms/routes/products.js)
* [Add new product](cms/routes/products.js)


### More features will be added to CMS soon...

## Workflow

### Authentication 
Authentication is pretty handy & simple, `auth/register` and `auth/login` are responsible for it. Once user is either registered or logged in, our system will generate a JWT in `x-auth-token` header.
<br/>
In order to register an admin user, you need to provide an acceptable JWT in `x-admin-token` with `SUPER_ADMIN` privileges.