# Domain Context Mapping

## 1. Patient Management

**Bounded Context:** Patient Management

**Primary Entities:**

* Patient
* Doctor
* Appointment
* Medical Record

## 2. Billing & Insurance Claims

**Bounded Context:** Billing & Insurance Claims

**Primary Entities:**

* Invoice
* Payment
* Insurance Policy
* Insurance Claim

## 3. Lab Test Diagnostics

**Bounded Context:** Lab Test Diagnostics

**Primary Entities:**

* Lab Test
* Test Order
* Sample
* Test Result

## Context Diagram

```mermaid
flowchart LR

    PM["Patient Management<br/>Patient<br/>Doctor<br/>Appointment<br/>Medical Record"]

    BC["Billing & Insurance Claims<br/>Invoice<br/>Payment<br/>Insurance Policy<br/>Insurance Claim"]

    LTD["Lab Test Diagnostics<br/>Lab Test<br/>Test Order<br/>Sample<br/>Test Result"]
```
