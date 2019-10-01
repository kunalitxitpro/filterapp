# README

Shopify Filter, Search and Infinite Scroll App

How to get the app running:

* Get an ngrok server pointing to localhost 3000

* Change the ngrok asset host to the ngrok address eg. config.action_controller.asset_host = "https://42c86952.ngrok.io"

* In the app configuration on Shopify set the admin redirect url to the ngrok address and change the proxy to the address but with the extension shopifyapp/products

* Run rake jobs:add_and_update_products (to get a local copy of the products)

* In the admin app set true and true filter to true

* The script will also then convert the shopify links to point to the proxy where the user filter products on all collection pages

* Testing can be done by visiting the shopify url with the proxy set on /apps/products or by also including a collection such as /apps/products/shorts
