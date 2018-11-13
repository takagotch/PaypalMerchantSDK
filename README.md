### PaypalMerchantSDK
---
https://github.com/paypal/merchant-sdk-dotnet/tree/master/PayPalMerchantSDK

```
<paypal>
<settings>
  <add name="mode" value="sandbox"/>
  <add name="connectionTimeout" value="30000"/>
</settings>
<accounts>
  <account apiUsername="jb-us-seller_api1.paypal.com" apiPassword="..." apiSignature="..."/>
  <account apiUsername="enduser_biz_api1.gmail.com" apiPassword="..." apiCertification="..." privateKeyPassword="..."/>
</accounts>
</paypal>
```
```
Dictionary<string, string> config = new Dictionary<string, string>();
config.Add("mode", "sandbox");
config.Add("account1.apiUsername", "jb-us-seller_api1.paypal.com");
config.Add("account1.apiPassword", "...");
config.Add("account1.apiSignature", "...");
PaypalAPIInterfaceService s = new PayPalAPIInterfaceService(config);

```

```ruby
account1.apiUsername = jb-us-seller_api1.paypal.com
account1.apiPassword = XXX
account1.apiSignature = XXXXX
account1.applicationId = APP-XXXX

account2.apiUsername = certuser_biz_api1.paypal.com
account2.apiPassword = XXXX
account2.apiCertificate = resource/sdk-cert.p12
account2.privateKeyPassword = password
account2.applicationId = APP-XXX

http.ConnectionTimeOut = 5000
http.Retry = 2
http.ReadTimeOut = 30000
http.MaxConnection = 100
http.IPAddress=127.0.0.1

mode=sandbox
service.RedirectURL = https://www.sandbox.paypal.com/webscr&cmd=
service.RedirectURL = https://www.paypal.com/webscr&cmd=
service.DevCentralURL=https://developer.paypal.com
sandbox.EmailAddress = pp.devtools@gmail.com
```




