# ECSNAP

flowchart LR
    A[User] -->|Opens EZSNAP App| B[Mobile App (Front End)]
    B -->|AR Try-On| C[AR Engine (ARKit / ARCore)]
    B -->|Fetch/Send Data| D[Backend Server & Database]
    D -->|Handles Inventory & Users| E[(Clothing Inventory)]
    D -->|Reservation Data| F[(Smart Lockers & Kiosks)]
    D -->|Photo Booth Access| G[(Photo Booth)]
    
    B -->|Payment Deposit| H[Payment Gateway]
    H -->|Deposit Refund| B
    
    G -->|Print Photos & Upload Digital Copy| B
    B -->|Shares Photos| I[Social Media]
    
    style A stroke:#333,stroke-width:2px,fill:#fff
    style B stroke:#27ae60,stroke-width:2px,fill:#eaffea
    style C stroke:#2980b9,stroke-width:2px,fill:#e7f1fa
    style D stroke:#8e44ad,stroke-width:2px,fill:#f4e7fa
    style E stroke:#f1c40f,stroke-width:2px,fill:#fdf8e3
    style F stroke:#c0392b,stroke-width:2px,fill:#fdecee
    style G stroke:#e67e22,stroke-width:2px,fill:#fdf2e6
    style H stroke:#2ecc71,stroke-width:2px,fill:#eaffea
    style I stroke:#3498db,stroke-width:2px,fill:#e7f1fa
