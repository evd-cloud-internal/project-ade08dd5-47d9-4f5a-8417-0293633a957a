---
name: Italy Article 6 2026-02-25
assetId: 6004f242-8f08-4867-be6b-66ce06d9f5b7
type: page
---

# Italy – Article 6 (Decreto-legge 20 febbraio 2026, n. 21)
## ETS Cost Compensation for Gas-Fired Generators
**Legal Assessment, Market Reaction & Likelihood of Approval**

---

## Introduction

On the 13th of February elements of Atricle 6 decree were leaked to Bloomberg and they reported that Rome was preparing a multi-billion-euro energy intervention affecting electricity pricing and carbon cost pass-through. On the 20th of February, the Italian government formally published *Decreto-legge n. 21/2026*, introducing a package of energy measures including Article 6, which establishes a mechanism to refund certain gas system charges and compensate gas-fired electricity generators for EU ETS compliance costs, subject to approval by the European Commission under EU State aid rules.


---

## 1. What Article 6 Does

Article 6 establishes a mechanism—effective from **1 January 2027**—that:

1. Extends **refunds of certain gas transport/system charges** applied to gas used for electricity generation.
2. Introduces an **additional refund mechanism linked to EU ETS compliance costs**, capped at the expected ETS compliance cost of an efficient combined-cycle gas turbine (CCGT) plant.
3. Explicitly states that the ETS-linked refund will only take effect **subject to approval by the European Commission under Article 108(3) TFEU** (State aid notification requirement).

Importantly, the measure does **not** amend EU ETS obligations. Gas generators remain legally obliged to monitor emissions and surrender allowances; the proposal instead seeks to offset compliance costs through a regulated compensation mechanism.

---

## 2. Market Reaction: Cal-27 Italian Baseload

```sql cal27_price
select
    toDate(Date) as date,
    argMax(Close, Time) as close
from italy_cal_27
group by date
order by date
```

{% line_chart
    data="cal27_price"
    x="date"
    y="close"
    title="Cal-27 Italian Baseload (€/MWh)"
    y_fmt="num2"
    x_sort="data"
    y_axis_options={
        fit_to_data=true
    }
    chart_options={
        zoom=true
    }
/%}

The Cal-27 Italian baseload contract was trading broadly range-bound around **€93/MWh** prior to 13 February. On the 13th of February after the leak was published by Bloomberg, the contract sold off sharply and found support around the **€86/MWh** region.

The initial weakness was followed by a pronounced rebound across 18–20 February, with prices climbing back above €91/MWh as regulatory uncertainty and implementation risk were priced in by the market. After the EU responded to the Italian decree the market saw more bearsih moves - although this time much more muted and the contract is now trading around **€89/MWh**.

---

## 3. The EU is fighting back

In January 2026 the European Commission opened six new infringement procedures against Italy—including on environmental law—highlighting Brussels’ heightened scrutiny of Rome’s compliance with EU law.

In February 2026 the Commission also launched a formal investigation into Italy’s so-called “anti-ETS” energy decree to assess its compatibility with EU rules after Rome’s attempt to decouple ETS costs from power prices drew attention in Brussels.

Together, these developments reinforce that measures affecting ETS implementation or electricity-market price formation are likely to face rigorous legal assessment at EU level.

---

## 4. Can Italy Do This Under EU Law?

### 4.1 ETS Obligations Cannot Be Altered Nationally

Under the EU Emissions Trading System (EU ETS):

- Installations must surrender allowances corresponding to verified emissions.
- Member States cannot unilaterally waive or reduce ETS compliance obligations.

Italy therefore cannot “remove” ETS costs in legal terms—it can only attempt to **offset them financially** via national measures.

---

### 4.2 State Aid Considerations (Article 107–108 TFEU)

Because Article 6 provides a financial advantage to a specific category of undertakings (gas-fired generators), funded or mandated via regulated mechanisms, it is highly likely to qualify as **State aid** under Article 107(1) TFEU.

As a result:

- The measure must be **notified to the European Commission**.
- It cannot be implemented until the Commission grants approval.
- The Commission will assess compatibility with the internal market.

The decree itself acknowledges this by conditioning implementation on Article 108(3) TFEU approval.

---

### 4.3 Structural Concerns

Key legal risks include:

- Weakening of the ETS carbon price signal.
- Distortion of wholesale electricity price formation.
- Competitive distortions within the internal market.
- Tension with EU decarbonisation objectives.

Existing ETS State aid frameworks focus primarily on **indirect cost compensation for energy-intensive industry**, not on compensating fossil fuel generators for direct compliance costs—making Article 6 comparatively novel and legally sensitive.

---

### 5. Conclusion

I think it is highly unlikely that the European Commission will approve Article 6 in its current form. At its core, the measure seeks to dilute the carbon price signal embedded in the EU ETS, a mechanism that sits at the centre of the EU’s decarbonisation strategy and its broader industrial policy. The ETS is not only a climate instrument; it is also designed to drive capital allocation, stimulate clean investment, and support Europe’s re-industrialisation through predictable carbon pricing.

By compensating gas-fired generators for ETS compliance costs, Article 6 risks weakening that price signal and undermining the “polluter pays” principle. It may also distort forward price formation in the wholesale electricity market, thereby affecting long-term investment signals for both generation and demand. This is particularly important given the EU is trying to mobilise record levels of private and public capital to develop grid infrastructure, renewable generation, flexibility assets, and electrification.

Whilst a modified (or temporary) version could potentially be negotiated, I believe that approval of Article 6 in its current structure would represent a significant departure from established EU climate and State aid principles, and therefore remains unlikely.





