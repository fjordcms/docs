# Authorization/authentication
Autorizace i autentizace je silně vázaná se systémem práv a celkového fungování uživatelského prostředí ve FjordCMS.

## Uživatel

User is anyone, who is registered on that website regardless his role, permissions or something else. User (entity) has 
only authentication and mandatory personal data. Other data not specific to this are added by custom or official (UserProfile link)
module extensions for this purpose.

Hierarchy of user: (What user has)
- User:
    - Data/details
        - Mandatory personal data
        - Authentication details
    - User-specific permissions
    - Roles
        - Permissions of that role
    - Archive in history of changes and actions
    
## Autentizace
Authentication or verifying user identity is managed by built-in authentication system. In default state, it's implemented only in administration part of system.

## In-fjord authentication system
Built-in authentication system in FjordCMS solving the problem of secure login (include two-factor authentication) without other features (solution of forgot password, registration) included in modules like UserProfile.
In case of use in administration (by default) there is registration solved by super-user creating user-account with pre-generated password (then that administration can change it)

### Dvoufázové ověření
Two-factor authentication is optional and is solved by sending one time verification code on selected E-mail.

## Autorizace
Authorization (verifying user permissions and roles) is solved by complex system of roles and perms.
In the end state, we however only see user permissions like sum of every perm he has (from roles, his or heredity) consisting of permission nodes.

What can authorization?
- Templates:
  - Clientside: restrict access to selected pages/forms/views or generate specific content for unauthorized user.
  - Adminside: restrict changes of specific settings or views for unauthorized administrators
- Modules:
  - Adminside: same as templates, settings
- Core:
  - preset permissions for example: allowing for access to administration