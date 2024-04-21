# eCommerceConnect plugin for WordPress (WooCommerce versions >= 8.3 with block support) for Ukraine

## Dependencies
- Requires WordPress at least: 6.3
- Tested up to: 6.4
- WC requires at least: 8.3
- WC tested up to: 8.6
- Requires PHP: 7.4

### Compatibility
This extension is compatible with:
- [WooCommerce Blocks](https://woo.com/document/cart-checkout-blocks-status/)

### Activation
Before using the extension, you need to apply for Internet acquiring from Ukrainian Processing Center

### Installation and configuration
1. Unzip the UPC extension (wordpress-woocommerce-8.3ua .zip > Unzip) and download the folder woocommerce-ecommerceconnect-gateway manually to the wp-plugins folder. 
Go to the admin panel.

2. In the menu Plugins once downloaded, click Install and Activate the plugin eCommerceConnect Gateway
![eCommerceConnect Gateway](image-1.png)

Go to WooCommerce > Settings and the Payments tab. Find eCommerceConnect in the list of extensions and click Manage
![WooCommerce](image-2.png)

3. Generate the public / private key pair with merchant crt according to the instructions from Ukrainian Processing Center
4. Copy the PEM key file to the server:

   Sandbox: wp-content/plugins/woocommerce-ecommerceconnect-gateway/cert/test/
   
   Prod: wp-content/plugins/woocommerce-ecommerceconnect-gateway/cert/prod/
   
5. Provide the *Callback URL* to the Ukrainian Processing Center to enable online payment notifications   
![notify url](image.png)

7. Enable *Sandbox* mode in the plugin settings
8. Disable *Sandbox* mode when ready to accept live payments
9. Merchant ID, Terminal ID fields are required
