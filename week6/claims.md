## Claims

Claims are name value pairs that shows what the subject is not what it can do. It represents a single fact about the user.
An Identity can be assigned to claims issued by a trusted party. Claims check the value of a claim and allows access to a resource. Claims can be a statement about or a property of an identity. A principal can have more than one identity and the identity can have more than one claim. The ClaimsPrincipal inherits all the claims of its identities.
**Claim Checks**  
Claims are embedded against a controller or an action within a controller. To add one, we building and register in the startup under the ConfigureServices().
**Authentication vs Authorization**  
*Authentication:*  
 - who you are
 - claim statements are about what or who you are, not what they can do
 - Identity has claims associated with it. Like Name, email, birthdate
 - 
*Authorization:* what you are allowed to do. 