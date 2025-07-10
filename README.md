# IronPaws
Created IronPaws, a mock defense tech app secured with Okta IdP and MFA to control a robotic dog access under Zero Trust principles.
##Features 
User authentication and authorization via Okta OpenID Connect (OIDC)  
- Role-based access control with custom user roles (e.g., Robotic Dog Operator)  
- Custom login page with IronPaw branding  
- Dynamic dashboard UI adapting to user roles  
- Secure session management and logout

## Why I Created This 
ZTA or Zero Trust Architecture is a security frame work that is ubqitious across different technical industries. This project demonstrates my ability to intrgrate the OKTA platform with an emphasis on tactical operational scenearios. 
## Getting Started

### Prerequisites

- Python 3.x  
- Virtual environment tool (venv or virtualenv)  
- Okta Developer account and application configured  

## Security Configuration Summary
This project includes basic Zero Trust access controls by integrating Okta with group-based policies and MFA enforcement. Specifically:

Tactical K-9 Unit Access Group
A custom Okta group named Tactical-K9-Unit was created to simulate access for high-security users (e.g., drone operators).

Strong Authenticator Requirement
A policy was created targeting the Tactical-K9-Unit group that requires use of a strong authenticator, such as Okta Verify. This ensures elevated accounts have phishing-resistant authentication.

MFA Enforcement Rule
An Okta sign-on rule was added to enforce MFA every login, not just once per session, for members of this group.

