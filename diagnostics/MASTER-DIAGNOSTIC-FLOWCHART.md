# MASTER DIAGNOSTIC FLOWCHART
## 2008 Mini Cooper S R56 - N14 Engine

This is the main diagnostic entry point. Follow symptoms to specific diagnostic guides.

---

## Quick Symptom Index

### 🔴 **CRITICAL/EMERGENCY SYMPTOMS**
| Symptom | Most Likely Cause | Diagnostic Guide |
|---------|------------------|------------------|
| **Air/hissing sound after 4000 RPM + power loss + won't start** | **Boost system catastrophic failure** | **[boost-leak-no-start-diagnosis.md](boost-leak-no-start-diagnosis.md)** |
| Loud rattling from engine (cold start) | Timing chain tensioner failure | [timing-chain-diagnosis.md](timing-chain-diagnosis.md) |
| Sudden loss of power, won't rev | High Pressure Fuel Pump failure | [HPFP-diagnosis.md](HPFP-diagnosis.md) |
| Overheating, coolant loss | Thermostat housing crack, water pump | [overheating.md](overheating.md) |
| Engine won't start, no crank | Battery, starter, or electrical | [no-start.md](no-start.md) |
| Engine won't start, cranks | Fuel pump, HPFP, ignition system | [no-start.md](no-start.md) |

---

## Diagnostic Flowchart by Symptom Category

### 1️⃣ **ENGINE NOISES**

```
RATTLING NOISE (Cold Start)?
├─ YES → Timing chain tensioner failure (CRITICAL)
│         → See: timing-chain-diagnosis.md
│
├─ Metallic rattling from transmission area?
│  └─ Dual-mass flywheel failure
│     → See: clutch-issues.md
│
├─ Rattling from turbo area (load)?
│  └─ Wastegate rattle or loose heat shield
│     → See: turbo-diagnosis.md
│
└─ Ticking/clicking from engine?
   └─ Low oil, lifter noise, or injector noise
      → Check oil level FIRST
      → See: oil-system.md
```

**Related Diagnostics:**
- [Timing Chain Diagnosis](timing-chain-diagnosis.md)
- [Turbo Problems](turbo-diagnosis.md)
- [Oil System Issues](oil-system.md)

---

### 2️⃣ **POWER LOSS / PERFORMANCE ISSUES**

```
SUDDEN COMPLETE POWER LOSS?
├─ Engine runs but won't rev past 2000 RPM?
│  └─ HPFP (High Pressure Fuel Pump) failure
│     → See: HPFP-diagnosis.md
│
├─ Limp mode (reduced power + check engine light)?
│  ├─ Boost control issues
│  │  → See: boost-problems.md
│  ├─ Turbo bypass valve failure
│  │  → See: turbo-diagnosis.md
│  └─ MAF sensor failure
│     → See: electrical-problems.md
│
└─ Gradual power loss?
   ├─ Carbon buildup on intake valves
   │  → See: carbon-buildup.md
   ├─ Clogged air filter
   └─ Boost leak
      → See: boost-problems.md
```

**Related Diagnostics:**
- [HPFP Diagnosis](HPFP-diagnosis.md)
- [Boost Problems](boost-problems.md)
- [Turbo Diagnosis](turbo-diagnosis.md)

---

### 3️⃣ **OIL CONSUMPTION / LEAKS**

```
OIL CONSUMPTION?
├─ Losing 1 quart per 1000 miles or more?
│  └─ NORMAL for N14 (but monitor closely)
│     → See: oil-system.md
│
├─ Blue smoke from exhaust?
│  ├─ Turbo seal failure
│  │  → See: turbo-diagnosis.md
│  └─ Piston ring wear
│     → Compression test needed
│
└─ Oil leak visible under car?
   → IDENTIFY LEAK SOURCE:
   ├─ Valve cover gasket
   ├─ Oil pan gasket
   ├─ Front/rear main seal
   ├─ Oil filter housing
   └─ Turbo oil feed/return lines
      → See: oil-system.md
```

**Related Diagnostics:**
- [Oil System Issues](oil-system.md)
- [Turbo Diagnosis](turbo-diagnosis.md)

---

### 4️⃣ **COOLANT LEAKS / OVERHEATING**

```
COOLANT LEAK?
├─ Leak from left side of engine?
│  └─ Thermostat housing crack (VERY COMMON)
│     → See: thermostat-housing-leak.md
│
├─ Leak from front of engine?
│  └─ Water pump failure
│     → See: overheating.md
│
├─ Leak from radiator?
│  └─ End tank crack or hose failure
│     → See: coolant-leaks.md
│
└─ OVERHEATING?
   ├─ Check coolant level FIRST
   ├─ Thermostat failure (stuck closed)
   ├─ Water pump failure
   ├─ Air in system
   └─ Cooling fan not working
      → See: overheating.md
```

**Related Diagnostics:**
- [Thermostat Housing Leak](thermostat-housing-leak.md)
- [Overheating](overheating.md)
- [Coolant Leaks](coolant-leaks.md)

---

### 5️⃣ **STARTING PROBLEMS**

```
WON'T START?
├─ ⚠️ RECENT AIR/HISSING SOUND + POWER LOSS?
│  └─ BOOST SYSTEM FAILURE
│     → See: boost-leak-no-start-diagnosis.md
│
├─ No crank (no sound when turning key)?
│  ├─ Dead battery
│  ├─ Starter motor failure
│  ├─ Ignition switch
│  └─ Neutral safety switch (auto)
│     → See: no-start.md
│
├─ Cranks but won't fire?
│  ├─ No fuel smell → FUEL ISSUE
│  │  ├─ HPFP failure
│  │  └─ Fuel pump
│  │     → See: HPFP-diagnosis.md
│  │
│  └─ Fuel smell present → IGNITION ISSUE
│     ├─ Ignition coils
│     ├─ Spark plugs
│     └─ Cam/crank position sensors
│        → See: no-start.md
│
└─ Hard starting (long crank)?
   └─ HPFP weak but not failed
      → See: HPFP-diagnosis.md
```

**Related Diagnostics:**
- [Boost Leak + No Start (After Hissing/Power Loss)](boost-leak-no-start-diagnosis.md)
- [No Start Diagnosis](no-start.md)
- [HPFP Diagnosis](HPFP-diagnosis.md)

---

### 6️⃣ **BOOST / TURBO ISSUES**

```
BOOST PROBLEMS?
├─ ⚠️ AIR/HISSING SOUND + POWER LOSS + WON'T START?
│  └─ CRITICAL FAILURE - Stop immediately!
│     → See: boost-leak-no-start-diagnosis.md
│     → Possible causes:
│        - Bypass valve catastrophic failure
│        - Intercooler hose blowout
│        - Turbo compressor damage
│        - Wastegate stuck open
│
├─ No boost / laggy acceleration?
│  ├─ Bypass valve diaphragm torn (VERY COMMON)
│  │  → See: turbo-diagnosis.md
│  ├─ Boost leak
│  │  → Pressure test intercooler system
│  │  → See: boost-problems.md
│  └─ Wastegate stuck open
│     → See: boost-problems.md
│
├─ Overboosting?
│  └─ Boost control solenoid failure
│     → See: boost-problems.md
│
└─ Turbo whistle/whine?
   ├─ Normal? (Some turbo noise is normal)
   └─ Excessive? → Bearing wear
      → See: turbo-diagnosis.md
```

**Related Diagnostics:**
- [Boost Leak + No Start (CRITICAL)](boost-leak-no-start-diagnosis.md)
- [Turbo Diagnosis](turbo-diagnosis.md)
- [Boost Problems](boost-problems.md)

---

### 7️⃣ **CHECK ENGINE LIGHT**

```
CHECK ENGINE LIGHT ON?
├─ SCAN CODES FIRST (Required for diagnosis)
│  → Use OBD-II scanner
│
├─ Common N14 Codes:
│  ├─ P0300-P0304 → Misfire
│  │  → See: misfire-diagnosis.md
│  ├─ P0087 → Low fuel pressure (HPFP)
│  │  → See: HPFP-diagnosis.md
│  ├─ P0299 → Turbo underboost
│  │  → See: boost-problems.md
│  ├─ P0171/P0174 → Lean condition
│  │  → Boost leak or MAF issue
│  └─ P0340/P0345 → Cam position sensor
│     → See: electrical-problems.md
│
└─ Flashing check engine light?
   → ACTIVE MISFIRE (Don't drive!)
      → See: misfire-diagnosis.md
```

**Related Diagnostics:**
- [Check Engine Codes](check-engine-codes.md)
- [Misfire Diagnosis](misfire-diagnosis.md)
- [HPFP Diagnosis](HPFP-diagnosis.md)

---

## 🔧 **Diagnostic Tools Needed**

### Essential:
- OBD-II scanner (code reader)
- Multimeter
- Compression tester
- Flashlight
- Basic hand tools

### Advanced:
- Boost pressure gauge
- Fuel pressure gauge
- Borescope (carbon inspection)
- Smoke machine (leak detection)
- MINI/BMW diagnostic software (INPA, ISTA)

---

## 📋 **Preventative Maintenance Checklist**

### Before Problems Occur:

**CRITICAL (Do ASAP if not done):**
- [ ] Timing chain tensioner replacement (2007-2009 N14)
- [ ] Verify oil consumption rate

**Regular Maintenance:**
- [ ] Oil change every 5,000 miles (0W-40 synthetic)
- [ ] Check oil level weekly
- [ ] Carbon cleaning every 30,000 miles
- [ ] Spark plugs every 60,000 miles

**Preventative Replacements:**
- [ ] Vacuum pump at 80-100k miles
- [ ] Thermostat housing (at first sign of leak)
- [ ] Water pump at 80-100k miles
- [ ] Bypass valve inspection

---

## Related Component Documentation
- [Engine Components](../engine/N14-engine-components.md)
- [Turbo Components](../turbo-system/turbo-components.md)
- [Fuel System](../fuel-system/fuel-components.md)
- [Cooling System](../cooling-system/cooling-components.md)
- [Electrical System](../electrical/electrical-components.md)
- [Transmission](../transmission/transmission-components.md)
