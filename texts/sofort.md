# SOFORT

SOFORT is a third party means of payment by Klarna Group. To process SOFORT via the Saferpay JSON API a few things must be observed.

## <a name="sf-requirement"></a> Requirements

The handling of SOFORT payments with Saferpay requires:

*	A corresponding licence and thus the existence of a valid identification with a username and password for the Saferpay system.
*	Availability of at least one active Saferpay terminal via which payment can be carried out and availability of the associated Saferpay TerminalId.
*	A valid acceptance agreement for SOFORT must be present.

 For SOFORT activation Saferpay needs:
 
*	Your SOFORT Customer ID.
*	The SOFORT Project ID.
*	The SOFORT Project password (NOT the account password!).
*	The Currency your customers will purchase with SOFORT.
*	Your Saferpay Customer ID.
*	The ID of the Saferpay eCommerce Terminal SOFORT is to be added.

**Attention**: Please send the information to activate SOFORT to **service.saferpay@six-payment-services.com**.

## <a name="sf-newproject"></a> Create a new project for SOFORT

1. Log-in to your SOFORT member area. Choose „New project“ and click „Create project“. <br>
![alt text](https://raw.githubusercontent.com/saferpay/sndbx/master/images/sofort_create_project.png "Create project")

2. Set the radio button for „Classic project“ and click again „Create project“. <br>
![alt text](https://raw.githubusercontent.com/saferpay/sndbx/master/images/sofort_classic_project.png "Classic project")

3. In the next step specify general settings for the project. <br>
![alt text](https://raw.githubusercontent.com/saferpay/sndbx/master/images/sofort_general.png "General settings")<br />
<i class="glyphicon glyphicon-hand-right"></i> <b><u>Don't forget to deactivate the Test mode before going live!</u></b>

4. Then enter <b><u>your address</u></b>. <br>
![alt text](https://raw.githubusercontent.com/saferpay/sndbx/master/images/sofort_address.png "Address")

5. Specify the currency for your customer’s payments. <br>
![alt text](https://raw.githubusercontent.com/saferpay/sndbx/master/images/sofort_currency.png "Currency")

6. Enter your IBAN for receiving your customer’s payments. <br>
![alt text](https://raw.githubusercontent.com/saferpay/sndbx/master/images/sofort_iban.png "Bank account")

7. For processiing SOFORT payments via Saferpay enter the redirect links. <br>
![alt text](https://raw.githubusercontent.com/saferpay/sndbx/master/images/sofort_interface.png "Interface")<br /><i class="glyphicon glyphicon-hand-right"></i> Success link:  
*https://-USER_VARIABLE_0-paymentStatus=ok-USER_VARIABLE_2--USER_VARIABLE_3--USER_VARIABLE_4--USER_VARIABLE_5--SENDER_IBAN-*<br /><i class="glyphicon glyphicon-hand-right"></i> Abort link:  
*https://-USER_VARIABLE_0-paymentStatus=cancel*

8. Save and click the tab „Extended settings“ to complete the project settings. <br>
![alt text](https://raw.githubusercontent.com/saferpay/sndbx/master/images/sofort_extended.png "Extended settings")

9. Go to „Shop interface settings“ and enter timeout value and link. <br>
![alt text](https://raw.githubusercontent.com/saferpay/sndbx/master/images/sofort_timeout.png "Timeout")<br /><i class="glyphicon glyphicon-hand-right"></i> Timeout in seconds:  
*900*<br /><i class="glyphicon glyphicon-hand-right"></i> Timeout link:<br />*https://-USER_VARIABLE_0-paymentStatus=timeout*

10. Again click the tab „Extended Settings“ and choose „Notifications“. <br>
![alt text](https://raw.githubusercontent.com/saferpay/sndbx/master/images/sofort_notification.png "Notifications")

11. Click „Add new notification“ and add your email address to receive notification messages. <br>
![alt text](https://raw.githubusercontent.com/saferpay/sndbx/master/images/sofort_email.png "Email notification")

12. Save and complete with adding the notification URL. As method choose „POST“. <br>
![alt text](https://raw.githubusercontent.com/saferpay/sndbx/master/images/sofort_noturl.png "Notification URL")<br /><i class="glyphicon glyphicon-hand-right"></i> HTTPS URL:<br />*https://-USER_VARIABLE_1-*

13. Finally create a project password. Click again the tab „Extended settings“ and there „Passwords and hash algorithm“. <br>
![alt text](https://raw.githubusercontent.com/saferpay/sndbx/master/images/sofort_password.png "Project password")  

The settings for processing SOFORT via Saferpay are completed!

---
