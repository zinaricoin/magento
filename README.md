# magento
Here is the official Zinari plugin for Magento 2
Download plugin
Unzip archive inside magento installation root folder and change rights on extracted files accordingly to your root folder owner (for ex. chown -R /var/www/magento2/ www-data:www-data)
Run set of the commands with magento binary (located in bin folder inside magento installation root)
magento module:enable Zinari_Payment --clear-static-content
magento setup:upgrade
magento setup:static-content:deploy -f
magento cache:clean
After Installation go to Stores -> Configuration -> Sales -> Payment Methods -> Zinari Cryptocurrency Gateway Magento inside Magento Admin panel and click expand icon
In plugin settings near Test Mode, select No (https://api.zinari.org) or Yes (https://api.zinari.org)
Type in your trade agreement in Trade ID and token inside Token (those details are provided to you after every new store creation in the response and inside email)
Click Save Config button
Thats it! Your users can pay using cryptocurrency now!
