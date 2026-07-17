&#x20;                         

### **GENERATE - BLOG (MAIN)**



&#x20;                          Start

&#x20;                            │

&#x20;                            ▼

&#x20;                     Open Application

&#x20;                            │

&#x20;                            ▼

&#x20;                   User Login/Register

&#x20;                            │

&#x20;                            ▼

&#x20;                 Authentication Successful

&#x20;                            │

&#x20;                            ▼

&#x20;                 Display User Dashboard

&#x20;                            │

&#x20;                            ▼

&#x20;               Enter Blog Generation Details

&#x20;      (Topic, Tone, Audience, Word Count, etc.)

&#x20;                            │

&#x20;                            ▼

&#x20;                   Click Generate Blog

&#x20;                            │

&#x20;                            ▼

&#x20;                 Check Available Credits

&#x20;                            │

&#x20;                 ┌──────────┴──────────┐

&#x20;                 │                     │

&#x20;                 ▼                     ▼

&#x20;       Credits Sufficient?          No

&#x20;                 │                     │

&#x20;                Yes                    ▼

&#x20;                 │           Display "Insufficient Credits"

&#x20;                 │                     │

&#x20;                 ▼                     ▼

&#x20;           Call AI Service      Show Subscription Plans

&#x20;                 │                     │

&#x20;                 ▼                     ▼

&#x20;       AI Generates Blog      Purchase Plan (Stripe)

&#x20;                 │                     │

&#x20;                 ▼                     ▼

&#x20;          Save Blog to Database  Credits Updated

&#x20;                 │                     │

&#x20;                 ▼                     └──────────────┐

&#x20;           Deduct User Credits                         │

&#x20;                 │                                    │

&#x20;                 ▼                                    │

&#x20;       Display Generated Blog ◄───────────────────────┘

&#x20;                 │

&#x20;                 ▼

&#x20;        User Chooses an Action

&#x20;                 │

&#x20;     ┌───────────┼──────────────────────────────────────────────┐

&#x20;     ▼           ▼             ▼             ▼           ▼       ▼

&#x20;  Copy Blog  Download PDF  Expand Blog  Shorten Blog  Regenerate Delete Blog

&#x20;     │           │             │             │           │         │

&#x20;     └───────────┴─────────────┴─────────────┴───────────┴─────────┘

&#x20;                             │

&#x20;                             ▼

&#x20;                        Update History

&#x20;                             │

&#x20;                             ▼

&#x20;                            End











### **USER-AUTHENTICATION**



Start

&#x20; │

&#x20; ▼

Open Website

&#x20; │

&#x20; ▼

Register/Login

&#x20; │

&#x20; ▼

Validate Credentials

&#x20; │

┌─┴──────────────┐

│                │

▼                ▼

Invalid       Valid

│                │

▼                ▼

Show Error   Generate JWT

&#x20;                 │

&#x20;                 ▼

&#x20;         Generate Refresh Token

&#x20;                 │

&#x20;                 ▼

&#x20;           Redirect Dashboard

&#x20;                 │

&#x20;                 ▼

&#x20;                End











### **PURCHASE - CREDITS**



Start

&#x20; │

&#x20; ▼

Open Subscription Plans

&#x20; │

&#x20; ▼

Select Plan

&#x20; │

&#x20; ▼

Proceed to Stripe Payment

&#x20; │

┌─┴───────────────┐

│                 │

▼                 ▼

Failed        Successful

│                 │

▼                 ▼

Show Error   Add Credits

&#x20;                 │

&#x20;                 ▼

&#x20;         Save Payment History

&#x20;                 │

&#x20;                 ▼

&#x20;           Display Success

&#x20;                 │

&#x20;                 ▼

&#x20;                End







### **ADMIN - DASHBOARD**



Start

&#x20; │

&#x20; ▼

Admin Login

&#x20; │

&#x20; ▼

Validate Credentials

&#x20; │

&#x20; ▼

Open Dashboard

&#x20; │

&#x20; ▼

Choose Operation

&#x20; │

&#x20; ├── View Users

&#x20; ├── View Blogs

&#x20; ├── View Payments

&#x20; ├── View Deleted Users

&#x20; ├── View Feedback

&#x20; ├── View Issues

&#x20; ├── Resolve Feedback

&#x20; ├── Resolve Issues

&#x20; └── Manage Plans

&#x20;          │

&#x20;          ▼

&#x20;     Save Changes

&#x20;          │

&#x20;          ▼

&#x20;        Logout

&#x20;          │

&#x20;          ▼

&#x20;         End

