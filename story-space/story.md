# App Story-Space
## Story 1


```mermaid

flowchart TD
    Start[Homepage] -->|Select location| Supermarket[Supermarket]
    Start -->|Select product| ProductDetails
    Start -->|Access| SavedProducts[Saved Products]
    SavedProducts --> Start
    SavedProducts -->|Select Product| ProductDetails
    Supermarket -->|Observe| Categories[Categories]
    Categories -->|Observe| Products[Products]
    Products -->|Select product| ProductDetails[ProductDetails]
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

# Story 3
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
