<h1>Group Policy Management: Account Policies/Password Policy & Account Policies/Account Lockout Policy</h1>



<h2>Description</h2>
During this laboratory session, we will be learning about configuring account policies for password management and account lockouts in our default domain. This is a crucial aspect of security, as it provides an extra layer of protection. For instance, it is recommended to set a limit on the number of login attempts before an account gets locked, as this can deter brute force attacks.
<br />




<h2>Environments Used </h2>

- <b>Windows Server 2019</b> 


<p align="center">
To begin, navigate to the Server Manager Dashboard, then choose the "Tools" option and scroll down to select "Group Policy Management". <br/>
<img src="https://github.com/Rastallworth1/Group-Policy-Management-Account-Policies-Password-Policy-Account-policies-Account-Lockout-policy/blob/main/Screenshot%201.png"/>
<br />


<br />
Once you are in the Group Policy Management window, locate and select the "Default Domain Policy" option. When you click on it, a pop-up message will appear, warning you that any changes made will affect other areas. You can choose to click "OK" and, if you prefer, select the option "don't show this message again."<br/>
<img src="https://github.com/Rastallworth1/Group-Policy-Management-Account-Policies-Password-Policy-Account-policies-Account-Lockout-policy/blob/main/Screenshot%202.png"/>
<br />


<br /> To proceed, click on the "Settings" option located at the top of the screen. Then, scroll down until you come across the "Account Policies" section. Here, you can review your current policies and decide whether they align with your organization's needs. Depending on your internet settings, you might encounter another pop-up message. If that happens, simply close it. For the purposes of this lab, we will be modifying two settings: the maximum password age (which determines how long before a password expires) and the account lockout threshold (which determines the number of login attempts before an account is locked). Please note that the specific values for these settings may be predefined by your organization.  <br/>
<img src="https://github.com/Rastallworth1/Group-Policy-Management-Account-Policies-Password-Policy-Account-policies-Account-Lockout-policy/blob/main/Screenshot%203.png"/>
<br />


<br />
To edit these policies, right click on Default Domain Policy and select edit.  <br/>
<img src="https://github.com/Rastallworth1/Group-Policy-Management-Account-Policies-Password-Policy-Account-policies-Account-Lockout-policy/blob/main/Screenshot%204.png"/>
<br />


<br />
Be prepared to do a fair amount of clicking now. In the Group Policy Management Editor, double-click on "Policies" under the "Computer Configuration" section. Next, double-click on "Windows Settings," followed by "Security Settings," and then "Account Policies." From there, you will see the options for "Password Policy," "Account Lockout Policy," or "Kerberos Policy." As you can see, this involves a fair bit of navigation.   <br/>
<img src="https://github.com/Rastallworth1/Group-Policy-Management-Account-Policies-Password-Policy-Account-policies-Account-Lockout-policy/blob/main/Screenshot%205.png"/>
<br />



  <br />
Let's start with modifying the Password Policy. First, select "Password Policy," and then choose "Maximum Password Age." Here, you can make changes to the policy. For this lab, we will set it to 90 days. Ensure that "Define this policy setting" is selected, then click on "Apply" and "OK." By doing so, all domain accounts will have their passwords expire after 90 days. However, please note that the specific number of days may vary depending on your organization's policies. A general rule of thumb is anywhere between 30 to 90 days.  <br/>
<img src="https://github.com/Rastallworth1/Group-Policy-Management-Account-Policies-Password-Policy-Account-policies-Account-Lockout-policy/blob/main/Screenshot%206%2C%20pt%201.png"/>
<br />
<br />
<img src="https://github.com/Rastallworth1/Group-Policy-Management-Account-Policies-Password-Policy-Account-policies-Account-Lockout-policy/blob/main/Screenshot%206%20pt%202.png"/>
<br />


<br />
Next, we will edit the Account Lockout Policy. To do so, select "Account Lockout Policy," and then choose "Account Lockout Threshold." You will have the option to make changes here. For this lab, we will set it to 3 attempts. Again, make sure that "Define this policy setting" is selected, then click on "Apply" and "OK." This will set the maximum number of login attempts to 3 for all accounts in the domain.  <br/>
<img src="https://github.com/Rastallworth1/Group-Policy-Management-Account-Policies-Password-Policy-Account-policies-Account-Lockout-policy/blob/main/Screenshot%207.png"/>
<br />



<br />
Finally, let's verify that the changes we made have been saved. Go back to the original "Default Domain Policy" settings and you should see that the modifications have been applied. Please note that there may be other items that can be changed, and you can use the same steps to make additional modifications to the Account Lockout and Password Policies as needed.  <br/>
<img src="https://github.com/Rastallworth1/Group-Policy-Management-Account-Policies-Password-Policy-Account-policies-Account-Lockout-policy/blob/main/Screenshot%208.png"/>
<br />

 
  
  


<br />
This was a simple Active Directory Home Lab / Tutorial thats demonstrates the proper steps to change Account Policies/Password Policy & Account Policies/Account Lockout Policy<br/>
