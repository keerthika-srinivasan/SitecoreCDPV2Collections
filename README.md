# Sitecore CDP Postman Collection

I’ve started a collection based on the Sitecore documentation and examples they've provided. You can import it into Postman and use it when working with your own Sitecore CDP sandbox. I hope you find it useful, please share any feedback.

## Authentication
<p id="postman">To use the collection against your sandbox you need to authenticate, Sitecore CDP supports basic <a rel="noreferrer noopener" href="https://doc.sitecore.com/cdp/en/developers/sitecore-customer-data-platform--data-model-2-1/authentication-for-the-sitecore-cdp-rest-apis.html" target="_blank">authentication</a>. An API token is a unique key that Sitecore provides your organization to authenticate your services.</p>

<p id="postman">1. You need to obtain your client key and API token from Sitecore CDP, in the navigation pane, click System Settings -&gt; API Access. For basic authentication:</p>
<ul><li>Username = Sandbox API Access Client Key</li><li>Password = Sandbox API Token</li></ul>
<p>2. You will need to update the variables in the postman collection:</p>
<ul><li>apiKeyId = Sandbox API Access Client Key</li><li>apiKeySecret = Sandbox API Token</li></ul>

## Collections Variables
<p>Here is a list of current variables within the collection:</p>
<table><tbody><tr><td><strong>Variable</strong></td><td><strong>Description</strong></td><td><strong>Examples </strong></td></tr><tr><td>apiKeyId</td><td>Your Sandbox API Client Key</td><td></td></tr><tr><td>apiKeySecret</td><td>Your Sandbox API Token</td><td></td></tr><tr><td>apiEndpoint</td><td>All URLs referenced in the Sitecore CDP v2.1 API<br>data model begin with the following base URL:&nbsp;<code>https://{apiEndpoint}/v2</code></td><td>api-engage-eu.sitecorecloud.io</td></tr><tr><td>pointOfSale</td><td>A POS is a specific storefront your organization sells products. Sitecore CDP supports multiple storefronts certain requests need to target the correct storefront.</td><td>betaSpinAir</td></tr><tr><td>currencyCode</td><td>The type of currency used for requests. String value (3 letter ISO 4217).</td><td>"EUR", "USD", "GBP"</td></tr><tr><td>language</td><td>The language captured on each page the guest visited.</td><td>"EN", "FR", "DE"</td></tr><tr><td>channel</td><td>The channel captured on each page the guest visited.</td><td>"WEB", "MOBILE_WEB", "MOBILE_APP"</td></tr><tr><td>guestRef</td><td>The unique ID of the guest generated by Sitecore CDP.</td><td>guid</td></tr><tr><td>guestEmail</td><td>The email address for the guest.</td><td></td></tr><tr><td>identifiersProvider</td><td>The provider of the identifiers.</td><td>ProfileSystem</td></tr><tr><td>identifiersId</td><td>The ID of the identifiers.</td><td>guid</td></tr><tr><td>dataExtensionName</td><td>The data extension name.</td><td>extEmailPreferences</td></tr><tr><td>dataExtensionRef</td><td>The reference of the data extension.</td><td>guid</td></tr><tr><td>orderRef</td><td>The reference of the order.</td><td>guid</td></tr><tr><td>orderItemRef</td><td>The reference of the order item.</td><td>guid</td></tr><tr><td>orderContactRef</td><td>The reference of the contact on the order.</td><td>guid</td></tr><tr><td>orderConsumerRef</td><td>The reference of the consumer on the order.</td><td>guid</td></tr><tr><td>batchFlowsJobRef</td><td>The reference of the Batch flow.</td><td>guid</td></tr><tr><td>decisionModelDefinitionRef</td><td>The reference of the Decision Model Definition.</td><td>guid</td></tr><tr><td>decisionModelDefinitionRevision</td><td>The reference of the Decision Model Definition Revisions.</td><td>guid</td></tr><tr><td>decisionModelVariantRef</td><td>The reference of the Decision Model Variant.</td><td>guid</td></tr><tr><td>decisionModelVariantRevision</td><td>The reference of the Decision Model Variant Revision.</td><td>guid</td></tr><tr><td>connectionRef</td><td>The reference of the Connection.</td><td>guid</td></tr></tbody></table>
