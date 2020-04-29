## OAUTH

This allows users to login through different website credentials such as GitHub, LinkedIn, Facebook, etc.
To start, we would need to register an app with the service provider. We need to specify a name for the app and a redirect URI, the service provider will give a client ID and client secret that is used in authenitcation and token requests.
- Consumers -> requests to service provider authorization endpoint that authorizes the user
- Service provider authenticates user and prompts whether to authorize the consumer
- if the user authorizes, the SP goes back to the redirect URI with a temp access code
- The consumer calls the token endpoint to exchange the code for a permanent access token.
- SP grants access that is used to authenticate requests to protected resources

[Resource](https://www.jerriepelser.com/blog/authenticate-oauth-aspnet-core-2/)