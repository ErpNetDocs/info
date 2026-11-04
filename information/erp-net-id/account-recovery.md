# Troubleshooting and account recovery

Use this guide if you cannot complete your ERP.net ID registration, sign in to Operator.net, or access any other ERP.net instance you have been invited to.

The main entry point for this process is the **Account recovery** button on the login screen.

The system automatically identifies the current status of your account and sends the appropriate email with a recovery link, depending on whether you need to complete your registration, confirm an email address change, or reset your password.

## You registered but did not confirm your email address (your registration)

When you create an ERP.net ID account (through Operator.net for example), the system sends a confirmation email to the address you entered during registration. Submitting the registration form alone does not complete this process. The e-mail's subject is "Email Confirmation", sender is "notification@erpnet.info".

<img width="503" height="388" alt="image" src="https://github.com/user-attachments/assets/113ea279-c364-4ee1-898f-6e42f4d81184" />
<br>

You must follow the link in that message to confirm your email address and complete account activation. 

> [!WARNING]  
> The confirmation link (token) is valid for **24 hours**. If you do not use it within that time, you will need a new confirmation email.

1. Open your inbox and find the confirmation email. Check your spam or junk folder if necessary.
2. If the link was issued less than 24 hours ago, open it to confirm your email address.
<br>
<img width="407" height="373" alt="image" src="https://github.com/user-attachments/assets/4c0c97c9-5a98-464a-bab0-094a4b7ed549" />
<br>
3. After confirmation succeeds, return to Operator.net and sign in using your ERP.net ID email and password.

### If the email is missing or the link has expired

The registration exists but is not yet complete. The system is awaiting your email confirmation, so you can still resolve this yourself without contacting support.

1. On the sign-in page, select **Account recovery** button.
2. Enter the same email address you used during registration and submit the request.
3. Check your inbox for the email-confirmation email.

<img width="1328" height="568" alt="image" src="https://github.com/user-attachments/assets/9b0e41be-1ba3-4e94-94b4-6e8cb7035b95" />

> [!IMPORTANT]  
> The same steps apply to any other instance, not only to id.erp.net, when the user has had his e-mail address changed, by an administrator and the latter has not sent a "Confirm Email" invitation through the dedicated function. In this case the new e-mail address in the user's account becomes IsConfirmed = False, so he will have to request an "Email Confirmation" letter by himself.
> If the administrator has used "Confirm Email" function, the user will receive an "Email Confirmation" letter that has no expiration. But still the risk of losing the letter remains.

### If no new email arrives

- Check your spam or junk folder.
- Make sure you entered the address used during registration.
- Avoid submitting repeated requests in quick succession; email sending is rate-limited.
- If you no longer have access to that mailbox, contact support for assistance.


