# Domain Context Mapping

## Context Diagram

```mermaid
flowchart LR

    H["Healthcare System"]

    subgraph PM["Patient Management"]
        P["Patient"]
        D["Doctor"]
        A["Appointment"]
        M["Medical Record"]
    end

    subgraph BI["Billing & Insurance Claims"]
        I["Invoice"]
        PAY["Payment"]
        IP["Insurance Policy"]
        IC["Insurance Claim"]
    end

    subgraph LD["Lab Test Diagnostics"]
        LT["Lab Test"]
        TO["Test Order"]
        S["Sample"]
        TR["Test Result"]
    end

    H --- PM
    H --- BI
    H --- LD
```

## Primary Entities

### Patient Management

* Patient
* Doctor
* Appointment
* Medical Record

### Billing & Insurance Claims

* Invoice
* Payment
* Insurance Policy
* Insurance Claim

### Lab Test Diagnostics

* Lab Test
* Test Order
* Sample
* Test Result

```

```
