# Custom Endpoint

Define a custom **https** endpoint to recieve batch JSON file when clicking the send button in the batch \(only visible when this is enabled\).

![Send JSON button appears in batch when this is activated](../.gitbook/assets/image%20%2879%29.png)

### Endpoint

Endpoint needs to be HTTPS and support CORS \([Cross-Origin Resource Sharing](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS)\). The endpoint will recieve a POST with json data containing all the batch and recipe data. Useful if you want to start a brew session on a custom automated brewery. Could for example be a custom [IFTTT ](https://ifttt.com/)webhook.

