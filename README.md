# WorkHive - Fullstack Saas for managing organizations of any size

# Technical documentation :

## Tech stack :
- React 
- Next.JS
- TailwindCSS
- Zustand
- Zod
- React hook form
- Postgres with neon
- Prisma as ORM
- Jwt
- Stripe

## Routes :
- For landing page `/`
- Login page `/login`
- Signup page `/signup`
- organization joining form `/join-org`

### **API overview**:
This project is leveraging nextjs api routes . The entire architecture is divided into these components :
#### accounts :
Refers to the **/account** parent route in apis . This parent route can handle all the   functionalities related to accounts
#### departments :
Refers to the **/department** parent route in apis . This route can handle all the   functionalities related to departments .
#### organizations :
Refers to the **/organization** parent route in apis . This route can handle all the   functionalities related to organizations .
#### tasks :
Refers to the **/tasks** parent route in apis . This route can handle all the   functionalities related to tasks .
#### notifications :
Refers to the **/notifications** route. While notifications creation is handled on where it's needed in entire apis, this route contains the delete route for handling notification delete 

### notes :
- Checkout payment webhook . Suspected a major level bug in the webhook route handling account creation .
- Create manager creation logic 
- The task can only contain comments with userEmail instead of userId
- Fix the theming of main dashboard of joined organization
- implement linkedin like tagging functionality in comments section 
- Remove emailing of link and implement functionality of handling invitations in notification panels of dashboard
- Add red dot when there is a notification in panel which is unseen
- Complete seening notification in frontend

test organizations:
abcbpo@gmail.com  jhDJ74@#

### Test accounts:

- amir465affan@gmail.com (jsDF34#$)
- ahmedabbasi903@gmail.com (jhFG@#23)
- aqiba.li82@gmail.com (jhFG76@#)
- aliabbasi@gmail.com (djDF56@#)
- affan.farooqsbf@gmail.com (dhFG@#87)

## Achieved:

###  **Schema overview :**
Before taking a look at schema , remember the following points.

- Each account have multiple organizations.
- multiple organizations belongs to same accounts.
- Each account have many notifications .
- many notifications belongs to same account
- Each organization have many departments
- many departments should belongs to same organization
- users should be joined in many departments
- task should be assignable to more than one users
- Each task should have many comments
- many comments should belong to one task


### **Features checklist**:
| Feature                                 | Status | tested |
| --------------------------------------- | ------ | ------ |
| Multi-auth system (login/signup)        | ✅     | ⬜    |
| Payments w/ Stripe                      | ✅     | ⬜    |
| Multi-org creation & management         | ✅     | ⬜    |
| Department system                       | ✅     | ⬜    |
| Invite system                           | ✅     | ⬜    |
| Task assignment to employees            | ✅     | ⬜    |
| Employee dashboard with task view       | ✅     | ⬜    |
| Task status update (done / in progress) | ✅     | ⬜    |
| Invitation and onboarding               | ✅     | ⬜    |
| 🔔 Notifications system ✅             | ✅     | ⬜    |
| Analytics dashboard                     | ⬜     | ⬜    |
| Notifications system                    | ✅     | ⬜    |
| Saas management dashboard               | ⬜     | ⬜    |
| guest mode in dashboard                 | ⬜     | ⬜    |
| Comments / collaboration                | ⬜     | ⬜    |
| Task relation like a related to b       | ⬜     | ⬜    |
| Manager creation feature                | ⬜     | ⬜    |
| Sicial login                            | ⬜     | ⬜    |
| Mobile responsive / PWA                 | ✅     | ⬜    |
| Role-based access control               | ⬜     | ⬜    |
| Live demo hosted                        | ⬜     | ⬜    |
| GitHub README with screenshots          | ⬜     | ⬜    |
| Blog/case study write-up                | ⬜     | ⬜    |