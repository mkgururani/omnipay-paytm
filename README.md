# omnipay-paytm

Use the following source code to communicate with the plugin

$gateway->setMerchantKey($merchantSecret->MerchantKey);

						$gateway->setTransactionAmount(<DONATION_AMOUNT>);
            
						$gateway->setChannelId($merchantSecret->ChannelId);
            
						$gateway->setIndustryType($merchantSecret->IndustryTypeId);
            
						$gateway->setMobileNum(<PHONE_NO>);
            
            $gateway->setEmail(<EMAIL_ID>);
							$gateway->setCustomerId(<CUSTMER_ID>);
						
						$gateway->setMID($merchantSecret->MID);
            
						$token = 'ODR-'.str_random(10);
            
						$gateway->setOrderId($token);
            
						$gateway->setWebsite($merchantSecret->Website);
            
						$gateway->setTestMode($isTestMode);
            
						$gateway->setCallBackUrl(<CALLBACK_URL
           
Add the following lines in composer.json file:

"repositories" : [{
			"type" : "composer",
			"url" : "https://packagist.org"
		},
		{
			"type" : "git",
			"url" : "https://github.com/mkgururani/omnipay-paytm",
			"reference": "master"
		}
	],
	"require-all": true,


This line must be included in "require" : { }
"omnipay-paytm" : "~0.1",
