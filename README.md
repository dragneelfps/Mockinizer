# Mockinizer
An OkHttpClient / RetroFit api call mocking library

## What is it?

Mockinizer helps Android developer to build apps with web api calls that use OkHttpClient / RetroFit by allowing them to quickly mock some web api responses with MockWebServer. Mockinizer allows to mock only specific api calls, while other api calls will still call the original server. 
This is particularily usefull in the following scenarios:
- You are working on a new feature that needs to call new not yet existing apis. With Mockinizer you can quickly swap in the new desired api responses while other api calls will still use the real server
- You want to test error cases for existing apis. With Mockinizer you can can quickly mock an error 500 response or an 401 Unauthorized for selected api requests and verify if your app handles them gracefully
- You want to call a mocked api for unit testing and isolate those from the webserver
