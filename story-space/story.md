# `Story-Space` and `FE Orchestration` for QRMeat
QRMeat is an app with the goal of informing users about the **details of the meat products** they consume, such as their origin and history. Thus, the primary aim of the app is reflected in its functionality, as the majority of interactions guide users towards the Products details page, as seen below.

## Story 1
```mermaid
flowchart TD
    Start[Homepage] -->|Select location| Supermarket[Supermarket]
    Start -->|Select product| ProductDetails
    Start -->|Access| SavedProducts[Saved Products]
    SavedProducts --> Start
    SavedProducts -->|Select Product| ProductDetails[Product Details]
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


## Story 2
```mermaid
flowchart TD
    Start[Homepage] -->|Access| News[News Page]
    News -->|Select| Article[Article]
    News -->|Scroll| News
    Article --> News
    News --> Statistics[Statistics]
    Statistics -->|Positive| Statistics
    Statistics -->|Negative| Statistics

```

### FE Orchestration

| Workflow   | Steps                                                                                          |
|:-----------:|:----------------------------------------------------------------------------------------------:|
|     1       | Access News Page → Scroll News → Select Article → Return to News Page → Access Statistics |
|     2       | Access News Page → Access Statistics                          |

