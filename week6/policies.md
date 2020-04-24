## Policies
Authorization policies have one or more requirements. IT was first have to be registered in the StartUp in the ConfigureServices Method within `services.AddAuthorization`. What determines if the authorization being successful with the IAuthorizationService.
To add policies to a Razor Page, you would just use the `[Authorize]` attribite with the kind of policy you would like to include such as if you want the user to be at least 21.  
You can create custom `iAuthorizationPolicyProvider`. It is useful if you use an external service for policy eval or use a lot of policies.  
**Authorization Requirements**   
These are collections of data parameters that policies can evaluate the user principal with. To make a requirement, it looks like you can make it using a class and it would need to inherit `IAuthorizationRequirement` interface. If there were more than one requirement, all of them would need to pass for the policy to succeed.  
**Authorization Handlers**  
In charge of the evaluation of the requirement properties to see if access if allowed. A requirement can have more than one handler. If a handler shows success, it calls `context.Succeed(IAuthorizationRequirement requirement)`. Handlers dont need to handle failures because other handlers might succeed. To make sure there is a fail, call `context.Fail`.