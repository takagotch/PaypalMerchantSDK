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


