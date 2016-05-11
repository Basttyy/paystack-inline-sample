# Paystack Inline Sample

Sample code that allows you quickly use Paystack inline on any page of your site. Note that this does not include a verify step.

## USAGE

### HTML Code

You may copy the code in [index.html](index.html).

At the very least, you will need to change the public key to your public key as provided here: https://dashboard.paystack.co/#/settings/developer .

### WordPress

To use on WordPress, download and install [wp-paystack-inline.zip](wp-paystack-inline.zip?raw=true) as a plugin on your Wordpress site.

* Configure the plugin on its settings page by adding your public key.

* Then include the shortcode: `[paystackinline costinnaira="NGN_AMT" message="MESSAGE"]` in the page/post where you want the payment form displayed.
    - Replace `NGN_AMT` with the amount in naira to be charged (all digits, no commas). 
        - Note that the cost is optional and a field will be provided for the customer to enter a value if it is not specified.
    - Replace `MESSAGE` with the message you want to display to your visitor after a successful payment. 
        - Note that the message is optional and a default of `You will also get a confirmation message in the mail.` will be displayed.
    
Valid samples include:
* `[paystackinline costinnaira="10400"]`
* `[paystackinline costinnaira="3000" message="Thanks for giving!"]`
* `[paystackinline message="Arigato!"]`
* `[paystackinline]`

