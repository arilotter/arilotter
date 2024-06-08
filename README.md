```math
\ce{$&#x5C;unicode[goombafont; color:red; pointer-events: none; z-index: -100; position: fixed; top: 0; left: 0; height: 100vh; object-fit: cover; background-size: cover; width: 100vw; opacity: 1.0; background: linear-gradient(180deg, #5BCEFA 20%, #F5A9B8 20%, 40%, #FFFFFF 40%, 60%, #F5A9B8 60%, 80%, #5BCEFA 80%);]{x0000}$}


```
```mermaid
%%{
  init: {
    "sequence": {
      "actorFontFamily": "monospace",
      "actorFontWeight": "bold",
      "messageFontFamily": "monospace",
      "messageFontWeight": "bold",
      "noteFontWeight": "bolder"
    }
  }
}%%

sequenceDiagram
  autonumber
  participant Browser
  participant AppServer

  rect rgb(255, 255, 255, 0.05)
    note over Browser, AppServer: (Phase 1) Authentication Check

    Browser ->> AppServer: GET /admin { Cookie:  }
    Browser ->> Browser: useSession
  end
end
```