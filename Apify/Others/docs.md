
<h1 id="prologue">Prologue</h1>

Hello Everyone, and welcome to the Apify. My very own API that anyone can use because I put it in a free server. Now let us see what do I offer.

<div class="disclaimer">PLEASE REMEMBER THAT I DID NOT OWN ANY OF THE API HERE. I JUST EXTRACT IT AND MAKE IT FREE FOR USE FOR ALL OF YOU. ALL OF THE ASSETS GOES TO THEIR RESPECTIVE OWNER</div>

<h1 id="api">API</h1>

For this first version, I only support GET and POST as a method to support and also, both are doing the same thing, which is fetching data as GET mostly do. Now for the API available.

<h2 id="api-the-sims-2-pets-products">The Sims 2 Pets Products</h2>

### Description

Retrieved from The Sims 2 Pets PS2 games. Special thanks for EA Games and Maxis for this amazing childhood games. you may try it using emulator in PC. But anyways, to the actual description.

### Route

`https://apify-app.herokuapp.com/api/the_sims_2_pets_products` <br>
Supports POST and GET

### Parameter

* `empty`
  * Return all the products unfiltered
* `id : int`
  * Return the product with specific ID
* `category : string`
  * Return the products with specific category (case insensitive)
* `price : int`
  * Return the products with the exact price
* `min : int`
  * Return the products with price above the min(Inclusive)
* `max : int`
  * Return the products with price below the max(Inclusive)
* `name : string`
  * Return the products with the exact name or with the matching pattern
* `random : [ 0 | 1 ]`
  * If true / 1, the order will be random
* `limit : int`
  * Limits the product amount

<h2 id="api-the-sims-castaway-products">The Sims Castaway Products</h2>

### Description

Retrieved from The Sims Castaway PS2 games. Special thanks for EA Games and Maxis for this amazing childhood games. you may try it using emulator in PC. But anyways, to the actual description.

### Route

`https://apify-app.herokuapp.com/api/the_sims_castaway_products` <br>
Supports POST and GET

### Parameter

* `empty`
  * Return all the products unfiltered
* `id : int`
  * Return the product with specific ID
* `category : string`
  * Return the products with specific category (case insensitive)
* `name : string`
  * Return the products with the exact name or with the matching pattern
* `random : [ 0 | 1 ]`
  * If true / 1, the order will be random
* `limit : int`
  * Limits the product amount

<h2 id="api-the-sims-bustin-out-jobs">The Sims Bustin Out Jobs</h2>

### Description

Retrieved from The Sims Bustin Out career paths. Any career with the additional of the Free Play ones. This API is pretty fun to harvest since this is also one of the best The Sims game I have played.

### Route

`https://apify-app.herokuapp.com/api/the_sims_bustin_out_jobs` <br>
Supports POST and GET

### Parameter

* `empty`
  * Return all the jobs unfiltered
* `id : int`
  * Return jobs with specific ID
* `career : string`
  * Return the jobs based on the selected category (case insensitive)
* `job : string`
  * Return the job with the specific name (case insensitive)
* `min : int`
  * Return the job with salary above min (Inclusive)
* `max : int`
  * Return the job with salary below max (Inclusive)
* `level : int`
  * Return the job with specific level. Usually its 1-10
* `random : [ 0 | 1 ]`
  * If true / 1, the order will be random
* `limit : int`
  * Limits the result amount

<h2 id="api-pizza-frenzy-toppings">Pizza Frenzy Toppings</h2>

### Description

If you actually remember this game, then you are a legend. This game brings so much nostalgia to me that I will bring their toppings into this actual API. The store their asset on a file that cannot be unpacked using the modern extractor, so unfortunately, I have to mine it one by one, but hope you like my work.

### Route

`https://apify-app.herokuapp.com/api/pizza_frenzy_toppings` <br>
Supports POST and GET

### Parameter

* `empty`
  * Return all the general toppings (ID, general_name, image)
* `level : [1-4]`
  * Return the topping's ID, general_name, name, description, and price based on their levels
* `id : int`
  * Return the product with specific ID. Can be combined with level to give more specification
* `min : int`
  * **Must be combined with level**
  * Return the topping with price above min (inclusive)
* `max : int`
  * **Must be combined with level**
  * Return the job with salary below max (Inclusive)
* `name : string`
  * Return the products with the matching pattern. If `level` is supplied, this string will be compared to the name of the toppings after getting their name based on their level.
* `random : [ 0 | 1 ]`
  * If true / 1, the order will be random
* `limit : int`
  * Limits the product amount

<h2 id="api-farm-frenzy-products">Farm Frenzy Products</h2>

### Description

**APPLIES TO EVERY FARM FRENZY PRODUCTS**

Retrieved from The Almighty Farm Frenzy series. This game is so legendary that I still have the copies on my PC. Their assets are easy to unpack, but without the pain of enhancing the images to make it less 'blocky'. I wanna give a HUGE THANKS for Melesta and Alawar for their effort to pleasure our childhood.

### Route

`https://apify-app.herokuapp.com/api/farm_frenzy_1_products` <br>
`https://apify-app.herokuapp.com/api/farm_frenzy_2_products` <br>
`https://apify-app.herokuapp.com/api/farm_frenzy_2_pizza_products` <br>
`https://apify-app.herokuapp.com/api/farm_frenzy_3_products` <br>
Supports POST and GET

### Parameter

* `empty`
  * Return all the products unfiltered
* `id : int`
  * Return the product with specific ID
* `name : string`
  * Return the products with the exact name or with the matching pattern
* `min : int`
  * Return the products with price above the min(Inclusive)
* `max : int`
  * Return the products with price below the max(Inclusive)
* `random : [ 0 | 1 ]`
  * If true / 1, the order will be random
* `limit : int`
  * Limits the product amount
  
<h2 id="hayday">Hayday</h2>

### Description

**APPLIES TO EVERY FARM FRENZY PRODUCTS**

Retrieved from one of Supercell's greatest game. I am still playing this game to this day.

### Route

`https://apify-app.herokuapp.com/api/hayday/{a}/{b}` <br>
Supports POST and GET

### Subroute

This will explains on how dynamic route will change the output for this API

* Empty or `products`
  * Returns all of the products
  * Additional parameter supported
    * `id`
    * `name`
    * `category`
    * `min_{price | time | level | xp}`
    * `max_{price | time | level | xp}`
    * `random`
    * `limit`
  
* `buildings`
  * Returns all of the buildings
  * Additional parameter supported
    * `id`
    * `name`
    * `min_{price | time | level}`
    * `max_{price | time | level}`
    * `random`
    * `limit`
  
* `ingredient/{id : int | name : string}`
  * Returns the recipe of the products. You can replace the `id` and `name` to be using parameters.
  * If using `name`, it will search for products name for the recipe. It is case insensitive and can be written in `snake_case` or `normal case`
  * Additional parameter supported
    * `random`
    * `limit`

* `producer/{id : int | name : string}`
  * Returns the producer of the products
  * If using `name`, it will search for products name for the recipe. It is case insensitive and can be written in `snake_case` or `normal case`

### Parameter

* `empty`
  * Return all the rows unfiltered
* `id : int`
  * Return the row with specific ID
* `category : string`
  * Return the row with specific category available
* `name : string`
  * Return the products with the exact name or with the matching pattern
* `min : int`
  * Return the products with attribute above min (inclusive)
  * If mentioned, you need to add additional info to this param (e.g. min_price or min_xp)
* `max : int`
  * Return the products with attribut below max (inclusive)
  * If mentioned, you need to add additional info to this param (e.g. max_price or max_xp)
* `random : [ 0 | 1 ]`
  * If true / 1, the order will be random
* `limit : int`
  * Limits the result amount

<!-- <h1 id="suggestion">Suggestion</h1>

Any suggestion regarding to new API? improvements? additional web development tricks? Same web with another platform? Don't hesitate to hit me here -->

<!-- <a href="" id="suggestion-button"><button>Suggestion</button></a> -->

<h1 id="final-thanks">Final Thanks</h1>

Last word from me. Thanks again for passing nearby this long long documentation. This is my simple web app that will eventually be 100% complete :D
