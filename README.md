graph TD
    %% Define Styles
    classDef trust fill:#2c3e50,stroke:#fff,stroke-width:4px,color:#fff,font-weight:bold;
    classDef holding fill:#1f77b4,stroke:#fff,stroke-width:2px,color:#fff,font-weight:bold;
    classDef subsidiary fill:#e1f5fe,stroke:#0277bd,stroke-width:1px,color:#000;
    classDef personal fill:#ffeb3b,stroke:#fbc02d,stroke-width:2px,color:#000;
    classDef personalEntity fill:#fff9c4,stroke:#fbc02d,stroke-width:1px,color:#000;

    %% --- TRUST STRUCTURE ---
    Trust(FAMILY TRUST):::trust
    TIA(Titanium Investments Africa Pty Ltd):::holding
    
    %% Relationships
    Trust -->|100%| TIA
    
    %% TIA Subsidiaries
    TIA -->|100%| SEG[SolarEnergyGroup Pty Ltd<br/><i>Dormant</i>]:::subsidiary
    TIA -->|100%| TEOA[The Energy of Africa Pty Ltd<br/><i>Trading</i>]:::subsidiary
    TIA -->|51%| Sone[Sone Contractors Pty Ltd<br/><i>Trading</i>]:::subsidiary
    TIA -->|50%| VTR[Vehicles to Rent Pty Ltd<br/><i>Trading</i>]:::subsidiary
    TIA -->|50%| SEL[Solar Energy Life Pty Ltd<br/><i>Dormant</i>]:::subsidiary
    TIA -->|49%| TA[TA Property Investments Pty Ltd<br/><i>Trading</i>]:::subsidiary
    TIA -->|30%| SGHW[Solar Guys Hot Water Solutions Pty Ltd<br/><i>Trading</i>]:::subsidiary

    %% --- PERSONAL HOLDINGS ---
    Me(TIHAN KUYPERS<br/>Personal Name):::personal
    
    %% Personal Entities
    Me -->|100%| Hatch[The Hatchery Business Concepts CC<br/><i>Trading as Solar Sales</i>]:::personalEntity
    Me -->|37%| Chicken[Chicken Country Retail CC<br/><i>Dormant</i>]:::personalEntity
    Me -->|33%| Glen[Glen Eden Trading 197 CC<br/><i>Sold</i>]:::personalEntity
    Me -->|26%| Ant[Ant Business Ventures CC<br/><i>Dormant</i>]:::personalEntity
    Me -->|Dir| Mod[Modimolle Silica Minerals Pty Ltd<br/><i>Closed</i>]:::personalEntity
    Me -->|Dir| PKG[PKG Promotions & Marketing Pty Ltd<br/><i>Dormant</i>]:::personalEntity
    Me -->|Dir| Adapt[Adaptive Incubation Pty Ltd<br/><i>Dormant</i>]:::personalEntity
    Me -->|Dir| Nyalowu[Nyalowu Investments Pty Ltd<br/><i>Inactive</i>]:::personalEntity
