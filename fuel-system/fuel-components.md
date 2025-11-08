# Fuel System Components - N14 Engine

## System Overview
The N14 uses a direct injection fuel system with high and low pressure circuits.

---

## Low Pressure System

### 1. **Fuel Tank**
**Capacity:** 13.2 gallons (50 liters)

**Components:**
- Fuel tank
- Fuel level sender
- In-tank fuel pump (low pressure)
- Fuel filter (in-tank)
- Rollover valves

---

### 2. **Low Pressure Fuel Pump**
**Location:** Inside fuel tank
**Pressure:** ~72 PSI

**Function:** Supplies fuel to HPFP

**Issues:**
- Weak pump (loss of power)
- Electrical connector corrosion
- Strainer clogging

---

## High Pressure System

### 3. **High Pressure Fuel Pump (HPFP)**
**Location:** Mounted on cylinder head, driven by exhaust cam
**Pressure:** 200-2,200 PSI (variable)

**Function:**
- Pressurizes fuel for direct injection
- Cam-driven mechanical pump with electronic control

**Common Failures:**
- Complete pump failure
- Pressure regulator failure
- Metal shavings contamination
- Seals/diaphragm failure

**Symptoms:**
- Hard starting (especially cold)
- Loss of power
- Rough idle
- Long crank times
- Limp mode

**Related:** `diagnostics/HPFP-diagnosis.md`

---

### 4. **Fuel Rail**
**Type:** High-pressure manifold
**Pressure:** Up to 2,200 PSI

**Components:**
- Fuel rail
- Fuel pressure sensor
- Pressure relief valve

---

### 5. **Fuel Injectors**
**Type:** Piezoelectric direct injectors (4)
**Location:** Cylinder head, side-mounted

**Function:**
- Inject fuel directly into combustion chamber
- Extremely fast response time

**Issues:**
- Carbon buildup on tips
- Electrical failure
- Seal leaks (fuel in oil)

---

### 6. **Fuel Pressure Sensor**
**Location:** Fuel rail

**Function:** Monitors high-pressure fuel pressure

---

## Evaporative Emissions System

### 7. **EVAP System**
**Components:**
- Charcoal canister
- Purge valve
- Vent valve
- Fuel tank pressure sensor

**Common Issues:**
- Check engine light (P0440-P0457 codes)
- Purge valve failure
- Leak detection pump failure

---

## Related Files
- [HPFP Diagnosis](../diagnostics/HPFP-diagnosis.md)
- [Fuel Pressure Testing](../diagnostics/fuel-pressure-test.md)
