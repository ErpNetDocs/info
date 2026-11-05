# Troubleshooting and account recovery

Use this guide if you cannot complete your ERP.net ID registration, sign in to Operator.net, or access any other ERP.net instance you have been invited to.

The main entry point for this process is the **Account recovery** button on the login screen.

The system automatically identifies the current status of your account and sends the appropriate email with a recovery link, depending on whether you need to complete your registration by confirming the email address or reset your password.

> [!NOTE]
> There are five User Types that conduct the interaction with the platform. A newly registered user is normally of type Invitation user (Invitation internal/Invitation external (No Login)), so the system needs to verify and then [change the type](https://docs.erp.net/tech/modules/system/security/ui-functions/change-user-type.html) to Internal user or External (community) user.

## You registered but did not confirm your email address (your registration)

When you create an ERP.net ID account (through Operator.net for example), the system sends a confirmation email to the address you entered during registration. Submitting the registration form alone does not complete this process. The e-mail's subject is "Email Confirmation", sender is "notification@erpnet.info".
<br>
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
<br>
<img width="1303" height="559" alt="image" src="https://github.com/user-attachments/assets/17f46d56-4cf3-40f5-a0f3-47aaa22821e3" />
<br>
3. Check your inbox for the email-confirmation email.
<br>

> [!IMPORTANT]  
> If the user has had his e-mail address changed, by an administrator, the new e-mail address in the user's account becomes IsConfirmed = False.<br>
> - The administrator has to send a "Confirm Email" invitation through the dedicated function - an "Email Confirmation" letter comes and expires in 24h.<br>
> - The user can still refer to "Account recovery" button for password reset, but will miss any letters if e-mail address remains unconfirmed.

## You forgot your password or want to change it

The system knows that your account is complete. In case you need to change or reset your password, the steps described above are applicable. The letter that you will receive is different - it focuses your password.

1. On the sign-in page, select **Account recovery** button.
2. Enter the same email address you used during registration and submit the request.
3. Open your inbox and find the letter "Reset your password for id.erp.net"
<br>
<img width="525" height="366" alt="image" src="https://github.com/user-attachments/assets/310fb1ca-792b-4432-a078-b8ac487239b0" />
<br>

> [!IMPORTANT]  
> The Reset password link is valid for 1 hour. You can still request another link at any time.<br>
> The same steps apply to any other instance.

## Multiple requests

The following rate limits apply to email sending (these limits were already in place and are not newly introduced):

- **Account recovery/invitation** – 3 emails **per user per hour**; 20 emails per IP address per hour.
- **Email confirmation resend** – 2 emails per user per minute; 20 emails per IP address per hour.

## If no new email arrives

- Check your spam or junk folder.
- Make sure you entered the address used during registration.
- Avoid submitting repeated requests in quick succession; email sending is rate-limited.
- If you no longer have access to that mailbox, contact support for assistance.


