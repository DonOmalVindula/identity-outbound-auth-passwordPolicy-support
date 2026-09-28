# Password Policy
The password policy enables you to force the user to reset the password in the authentication flow in the WSO2 Identity Server. This along with IS Analytics also enables sending notifications to users when the password had expired.

## Getting started
To get started with the password policy, go to [Configuring Password Reset Enforcer](config.md). Once you have completed your configurations you can make the users reset their password after a configurable time period and also send email notifications to login and change the password.

## Compatibility with WSO2 Identity Server 7.1.0
Connector v4.0.11 is compatible with WSO2 Identity Server 7.1.0 from update level UPDATE_LEVEL_TBD onwards. On earlier 7.1.0 update levels, use connector v4.0.9: v4.0.10 and later cannot complete a password reset on those update levels, and fail after the new password has already been saved.

Always deploy the connector JAR and the `pwd-reset.jsp` page from the same connector release. From v4.0.10 onwards the form fields of `pwd-reset.jsp` changed, so a JAR and a page from different releases do not work together.

## Additional information
To download the Password Reset Enforcer and other artifacts, go to [Password Reset Enforcer on WSO2 Store](https://store.wso2.com/connector/identity-outbound-auth-passwordPolicy)
