# E-mail management

E-mails in FjordCMS are managed with elegant way, thanks to which you only need to set up email accounts once in the whole system and then, in each module there is used dependency injection (module works with abstract interface of e-mail entity from FjordCMS core - email will be selected automatically or by client in module settings administration).
There is also paginated list of sent email in history for each email (even, if e-mail was deleted from).

### Required parameters for each email
- Name
- Server Host (SMTP)  
- Server Email (SMTP)
- Server Password (SMTP)
- Receiver Email

You can add multiple e-mail accounts named by your choice and then select what e-mail will be used in what module section (module can use different emails for different actions).