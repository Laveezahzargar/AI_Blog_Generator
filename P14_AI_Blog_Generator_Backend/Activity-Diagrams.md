1. User-Authentication:



&#x20;                          Start

&#x20;                            │

&#x20;                            ▼

&#x20;                     Open Application

&#x20;                            │

&#x20;                            ▼

&#x20;                   Register / Login

&#x20;                            │

&#x20;                            ▼

&#x20;                 Validate Credentials

&#x20;                            │

&#x20;                 ┌──────────┴──────────┐

&#x20;                 │                           │

&#x20;                 ▼                          ▼

&#x20;         Invalid Credentials        Valid Credentials

&#x20;                 │                           │

&#x20;                 ▼                           ▼

&#x20;         Display Error Message   Generate JWT \& Refresh Token

&#x20;                                             │

&#x20;                                             ▼

&#x20;                                    Save Refresh Token

&#x20;                                             │

&#x20;                                             ▼

&#x20;                                    Redirect to Dashboard

&#x20;                                             │

&#x20;                                             ▼

&#x20;                                            End





2\. Generate-Blog(Main-Workflow):



&#x20;                          Start

&#x20;                            │

&#x20;                            ▼

&#x20;                     Open Application

&#x20;                            │

&#x20;                            ▼

&#x20;                   Login / Register

&#x20;                            │

&#x20;                            ▼

&#x20;                 Authentication Successful

&#x20;                            │

&#x20;                            ▼

&#x20;                   Display User Dashboard

&#x20;                            │

&#x20;                            ▼

&#x20;              Enter Blog Generation Details

&#x20;     (Topic, Tone, Audience, Category , Word Count)

&#x20;                            │

&#x20;                            ▼

&#x20;                   Click Generate Blog

&#x20;                            │

&#x20;                            ▼

&#x20;                 Check Available Credits

&#x20;                            │

&#x20;                 ┌──────────┴──────────┐

&#x20;                 │                           │

&#x20;                 ▼                           ▼

&#x20;         Credits Sufficient?                 No

&#x20;                 │                           │

&#x20;                Yes                          ▼

&#x20;                 │               Display "Insufficient Credits"

&#x20;                 │                           │

&#x20;                 ▼                           ▼

&#x20;             Call AI Provider      Display Subscription Plans

&#x20;                 │                           │

&#x20;                 ▼                           ▼

&#x20;         AI Generates Blog            Purchase Plan (Stripe)

&#x20;                 │                           │

&#x20;                 ▼                           ▼

&#x20;         Save Blog to Database            Add Credits

&#x20;                 │                           │

&#x20;                 ▼                           │

&#x20;     Create Original Blog Version            │

&#x20;                 │                          │

&#x20;                 ▼                         │

&#x20;        Deduct User Credits ◄──────────┘

&#x20;                 │

&#x20;                 ▼

&#x20;        Display Generated Blog

&#x20;                 │

&#x20;                 ▼

&#x20;        User Chooses an Action

&#x20;                 │

&#x20;┌──────┬────────┬────────┬────────┬──────────┬────────────┬

&#x20;▼       ▼          ▼          ▼          ▼             ▼               ▼

Copy  Download     Expand     Shorten     Regenerate     Generate        Delete

Blog    PDF         Blog        Blog         Blog          Image          Blog

&#x20;│        │         │            │           │             │             │

&#x20;└──────┴──────  ┴───────    ┴───────┴──────────┴────────  ─┘

&#x20;                         │

&#x20;                         ▼

&#x20;            Save New Version (if applicable)

&#x20;                         │

&#x20;                         ▼

&#x20;                 Update Blog \& Version History

&#x20;                         │

&#x20;                         ▼

&#x20;                        End





3\. Purchase-Credits(Stripe):



&#x20;                          Start

&#x20;                            │

&#x20;                            ▼

&#x20;                Open Subscription Plans

&#x20;                            │

&#x20;                            ▼

&#x20;                     Select a Plan

&#x20;                            │

&#x20;                            ▼

&#x20;               Proceed to Stripe Checkout

&#x20;                            │

&#x20;                 ┌──────────┴──────────┐

&#x20;                 │                     │

&#x20;                 ▼                     ▼

&#x20;           Payment Failed      Payment Successful

&#x20;                 │                     │

&#x20;                 ▼                     ▼

&#x20;       Display Error Message    Save Payment Record

&#x20;                                       │

&#x20;                                       ▼

&#x20;                               Add Purchased Credits

&#x20;                                       │

&#x20;                                       ▼

&#x20;                         Create Credit Transaction

&#x20;                                       │

&#x20;                                       ▼

&#x20;                          Display Success Message

&#x20;                                       │

&#x20;                                       ▼

&#x20;                                      End



4\. Profile-Management:

&#x20;                          Start

&#x20;                            │

&#x20;                            ▼

&#x20;                     User Login

&#x20;                            │

&#x20;                            ▼

&#x20;                    Open Profile

&#x20;                            │

&#x20;                            ▼

&#x20;                   Choose an Action

&#x20;                            │

&#x20;    ┌───────────────┬────────────────┬────────────────┐

&#x20;    ▼               ▼                ▼        ▼                      ▼

Update Profile  Upload Picture  Delete Picture  Delete Account Change Password

&#x20;    │               │                │                │

&#x20;    └───────────────┴────────────────┴────────────────┘

&#x20;                            │

&#x20;                            ▼

&#x20;                     Save Changes

&#x20;                            │

&#x20;                            ▼

&#x20;                   Display Confirmation

&#x20;                            │

&#x20;                            ▼

&#x20;                           End



5\. Feedback and Issue Management:



&#x20;                          Start

&#x20;                            │

&#x20;                            ▼

&#x20;                       User Login

&#x20;                            │

&#x20;                            ▼

&#x20;                    Open Support Page

&#x20;                            │

&#x20;                            ▼

&#x20;                    Choose an Action

&#x20;                            │

&#x20;                ┌───────────┴───────────┐

&#x20;                ▼                       ▼

&#x20;         Submit Feedback          Raise Issue

&#x20;                │                       │

&#x20;                ▼                       ▼

&#x20;       Enter Feedback Details   Enter Issue Details

&#x20;                │                       │

&#x20;                └───────────┬───────────┘

&#x20;                            ▼

&#x20;                    Save to Database

&#x20;                            │

&#x20;                            ▼

&#x20;                 Display Confirmation

&#x20;                            │

&#x20;                            ▼

&#x20;                           End



6\. Admin-Dashboard:



&#x20;                          Start

&#x20;                            │

&#x20;                            ▼

&#x20;                       Admin Login

&#x20;                            │

&#x20;                            ▼

&#x20;                 Validate Credentials

&#x20;                            │

&#x20;                            ▼

&#x20;                Open Admin Dashboard

&#x20;                            │

&#x20;                            ▼

&#x20;             View Dashboard Statistics

&#x20;     (Users, Blogs, Payments, Credits, Feedback,Issues)

&#x20;                            │

&#x20;                            ▼

&#x20;                  Choose an Operation

&#x20;                            │

&#x20;┌─────────┬─────────┬──────────┬────────────┬───────────┬──────────┬

&#x20;▼           ▼             ▼             ▼               ▼              ▼             ▼

Users       Blogs       Payments Credit Transactions       Feedback         Issues      Deleted Users

&#x20;                                                         │               │

&#x20;                                                         ▼              ▼

&#x20;                                                   Resolve Feedback  Resolve Issues

&#x20;

&#x20;                                                       └───────────┬───────────┘

&#x20;                                                                   │

&#x20;                                                                   ▼

&#x20;                                                              Save Changes

&#x20;                                                                   │

&#x20;                                                                   ▼

&#x20;                                                                 Logout

&#x20;                                                                   │

&#x20;                                                                   ▼

&#x20;                                                                  End

