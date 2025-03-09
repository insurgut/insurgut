```mermaid
flowchart TB;
    %% Main node style
    classDef main fill:#1e1e1e,stroke:#ff5733,stroke-width:2px,color:#ffffff,font-weight:bold,rx:10,ry:10;
    classDef normal fill:#282828,stroke:#ff5733,stroke-width:2px,color:#ffffff,rx:8,ry:8;

    %% Define the main vertical blocks for PC Hardware
    subgraph PCHardware
        direction TB;
        P1["PC Components"]:::main;
        P1 --> P2["Intel i9-12Gen"]:::main;
        P1 --> P3["GIGABYTE Z790 AORUS ELITE"]:::main;
        P1 --> P4["RX 7800 XT, RTX 3050S"]:::main;
        P1 --> P5["Custom Water Cooling"]:::main;
        P1 --> P6["AULA 78R, SteelSeries Apex"]:::main;
    end

    %% Define the main vertical blocks for Lisurgut Info
    subgraph LisurgutInfo
        direction TB;
        L1["Lisurgut - User"]:::main;
        L1 --> L2["Languages: HTML, CSS, JS, Python"]:::main;
        L1 --> L3["Servers: Personal"]:::main;
        L1 --> L4["Focus: Gaming Setup"]:::main;
    end

    %% Connect the two blocks
    PCHardware -.-> LisurgutInfo;
