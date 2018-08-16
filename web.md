# Website

All dates are in the strftime format "%Y-%m-%d %H-%M-%S".
Currency amounts are in cents.

## acc_created

Table with the account creation date. In my case this data was incorrectly dumped.

* `accCreated`: Account creation date

## activities

Table with the activity feed displayed on your personal profile like started forum topics, achievements and milestones.

* `activity`: JSON data of activity
* `created_at`: Date of activity creation

## birth_date

Table with the date of birth. In my case this data was incorrectly dumped.

* `dataUrodzenia`: Date of birth

## forum_posts

Table with all forum posts.

* `thread_name`: Name of the thread
* `post_content`: Text of the post
* `post_date`: Date of the post

## order_products

Table assigning order IDs to product names.

* `public_id`: Order ID
* `title`: Title of the product

## orders

Table with orders. IPs in this file have been replaced with examples to save me from potential trouble.

* `status`: Unknown
* `public_id`: Order ID
* `date_created`: Date the order was created
* `date_paid`: Date it was paid or NULL
* `ip_address_created`: IP address the order was created from
* `ip_address_paid`: Always NULL in my case
* `base_amount`: Price of all products without discount
* `discount_amount`: Discount to subtract from the base price
* `tax_amount`: Amount of taxes paid
* `payment_amount`: Total amount paid including taxes excluding store credit
* `currency_code`: Currency code
* `store_credit_amount`: Store credit used for the payment

## payments

Table with payment amount and type.

* `public_id`: Order ID
* `method_slug`: Payment method slug. Known values: `pscard`, `sofort`, `paypal`
* `amount`: Amount paid
* `currency`: Currency code
* `payment_status`: Unknown

## products

Table with owned products and their order date.

* `game_title`: Title of the product
* `order_date`: Date the order was created

## profile_preferences

Table with profile privacy settings. Only known value is 3 for "all visitors".

* `privacy`: Who can see your profile
* `privacy_games`: Who can see your games list
* `privacy_friends`: Who can see your friends list

## subscriptions

Table with newsletter subscription dates.

* `info_subscriber`: Type of subscription. Known values:
    `info_subscriber` (Releases and Announcements),
    `promo_subscriber` (Promotions and hot deals),
    `wishlist_subscriber` (Wishlist alerts)
* `date_subscribed`: Date subscribed

## wishlist

Table with wishlist products and 

* `game_title`: Title of the product in lower case and with special characters removed
* `date_added`: Date added to wishlist
