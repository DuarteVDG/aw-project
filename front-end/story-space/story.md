# `Story-Space` and `FE Orchestration` for QRMeat

## Story 1
```mermaid
flowchart TD
    Start[Login] -->|Enter Credentials| Validate[Validate Credentials]
    Validate -->|Valid| Home[Home Page]
    Validate -->|Invalid| Error[Error Message]
    Home -->|View Profile| Profile[User Profile]
    Home -->|Logout| Start
    Profile -->|Edit Profile| Edit[Edit Profile]
    Profile -->|Change Password| Change[Change Password]
    Profile -->|Forgot Password| Forgot[Forgot Password]
    Profile -->|Create Account| Create[Create Account]
    Edit -->|Save| Profile
    Change -->|Save| Profile
    Forgot -->|Enter Email| Email[Enter Email]
    Email -->|Send Reset Link| ResetLink[Send Reset Link]
    ResetLink -->|Link Sent| Success[Success Message]
    ResetLink -->|Invalid Email| ErrorEmail[Error Message]
    Create -->|Enter Details| Details[Enter Details]
    Details -->|Create Account| NewAccount[Create Account]
    NewAccount -->|Account Created| Success[Success Message]
    NewAccount -->|Cancel| Start
```


## Story 2
```mermaid
flowchart TD
    Start[Homepage] -->|Select location| Supermarket[Supermarket]
    Start -->|Select product| ProductDetails[Product Details]
    Start -->|Access| SavedProducts[Saved Products]
    SavedProducts --> Start
    SavedProducts -->|Select Product| ProductDetails
    Supermarket -->|Observe| Categories[Categories]
    Categories -->|Observe| Products[Products]
    Products -->|Select product| ProductDetails
    ProductDetails -->|ExpandDetails|ProductDetails
    ProductDetails -->|View| Feedback
    Feedback -->|Save Product| Feedback
    Feedback -->|Give feedback| Feedback
    Feedback --> ProductDetails
    ProductDetails --> Products
    Supermarket -->|Access| QRCode[QR Code]
    QRCode -->|Observe| ProductDetails
    QRCode -->|Scan| QRCode
```

### FE Orchestration

| Workflow  | Steps                                                                                 |
|:-----------:|:-------------------------------------------------------------------------------------:|
|     1       | Select location → Observe Categories → Observe Products → Select product → View Product Details  → View Feedback → Save product → Give Feedback      |
|     2       | Select location → Access QR Code → Scan Product → Observe Product Details → View Feedback → Save product → Give Feedback |
|     3       | Select product → View Feedback → Save product → Give Feedback |
|     4       | Access Saved Products → Select product → View Feedback → Save product → Give Feedback |

**Note:** QRMeat is an app with the goal of informing users about the **details of the meat products** they consume, such as their origin and history. Thus, the primary aim of the app is reflected in its functionality, as the majority of interactions guide users towards the `Products Details` page, as seen above.




## Story 3
```mermaid
flowchart TD
    Start[Homepage] -->|Access| News[News Page]
    News -->|Select| Article[Article]
    News -->|Scroll| News
    Article --> News
    News  -->|Access| Statistics
    Statistics -->|Navigate| Statistics

```

### FE Orchestration

| Workflow   | Steps                                                                                          |
|:-----------:|:----------------------------------------------------------------------------------------------:|
|     1       | Access News Page → Scroll News → Select Article → Return to News Page → Access Statistics → Navigate Statistics|
|     2       | Access News Page → Access Statistics → Navigate Statistics                        |

