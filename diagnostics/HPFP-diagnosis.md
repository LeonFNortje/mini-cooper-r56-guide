# High Pressure Fuel Pump (HPFP) Diagnosis

## Overview

The HPFP is a **common failure point** on N14 engines. It's cam-driven and provides fuel at extremely high pressure (200-2,200 PSI) for the direct injection system.

---

## Symptoms of HPFP Failure

### Early/Intermittent Failure:
- ✓ Hard starting (especially cold)
- ✓ Long crank time (3-5+ seconds)
- ✓ Occasional hesitation
- ✓ Intermittent power loss
- ✓ Check engine light (may come and go)

### Progressive Failure:
- ✓ Harder to start each time
- ✓ Rough idle when cold
- ✓ Loss of power under load
- ✓ Hesitation when accelerating
- ✓ Won't rev past 2,000-3,000 RPM
- ✓ Limp mode

### Complete Failure:
- ✓ Engine won't start at all
- ✓ Cranks but never fires
- ✓ No fuel smell at exhaust
- ✓ Or: starts briefly then dies

---

## Diagnostic Steps

### Step 1: Check for Codes
**Use:** OBD-II scanner

**Related Codes:**
- **P0087:** Fuel rail pressure too low (PRIMARY CODE)
- P0088: Fuel rail pressure too high
- P0089: Fuel pressure regulator malfunction
- P2293: Fuel pressure regulator 2 performance
- P0090-P0094: Various fuel system codes

**Critical:** P0087 is the smoking gun for HPFP issues

---

### Step 2: Observe Starting Behavior
**Test:** Cold start the engine

**Procedure:**
1. Engine cold (sit overnight)
2. Turn key to ON (don't start)
3. Wait 2 seconds (prime fuel system)
4. Crank engine, count seconds to start

**Normal:** Starts in 1-2 seconds
**HPFP Issue:**
- Takes 3-5+ seconds
- Multiple cranks needed
- Gets worse over time

---

### Step 3: Monitor Fuel Pressure
**Requires:** Fuel pressure gauge or scan tool with live data

**Test:**
1. Connect pressure gauge to fuel rail test port
2. Start engine
3. Monitor pressure at idle and under load

**Normal Readings:**
- Idle: 500-700 PSI
- Part throttle: 1,000-1,500 PSI
- Full throttle: 1,800-2,200 PSI

**HPFP Failure:**
- Below 500 PSI at idle
- Drops below 1,000 PSI under load
- Unstable/fluctuating pressure

**Alternative:** Use BMW/MINI diagnostic software (INPA, ISTA)
- Read "Rail Pressure Actual" vs "Rail Pressure Desired"
- Large gap indicates pump failure

---

### Step 4: Check Low Pressure System
**Before condemning HPFP, verify low pressure fuel system**

**Test Low Pressure Pump:**
1. Turn key to ON (don't start)
2. Listen at fuel tank for pump humming (2 seconds)
3. Measure pressure at HPFP inlet

**Normal:** 72 PSI at HPFP inlet
**Low Pressure Issue:** Below 60 PSI

**Common Low Pressure Issues:**
- Weak in-tank fuel pump
- Clogged fuel filter
- Bad fuel pressure regulator

**Related:** [Fuel System Components](../fuel-system/fuel-components.md)

---

### Step 5: Visual Inspection
**Access:** HPFP is on top of engine, passenger side

**Check for:**
- ✓ External fuel leaks
- ✓ Oil contamination (rare)
- ✓ Electrical connector damage
- ✓ Mounting bolts loose
- ✓ Vacuum line to pressure regulator

---

### Step 6: HPFP Output Test (Advanced)
**Requires:** Mechanical aptitude, special tools

**Procedure:**
1. Disconnect HPFP outlet line
2. Crank engine (don't start)
3. Observe fuel output

**Normal:** Strong pulsing fuel flow
**Failed:** Weak or no fuel flow

**Warning:** High pressure fuel is dangerous - use caution

---

## Confirmation Tests

### Swap Test (If Available):
- Swap HPFP with known good unit
- If problem goes away → Confirms HPFP failure

### Fuel Quality Test:
- Bad fuel can kill HPFP
- Check for water in fuel
- Check for metal shavings (pump destruction)

---

## Decision Tree

```
LONG CRANK / HARD START?
│
├─ Scan shows P0087 code?
│  └─ YES → 90% likely HPFP failure
│     ├─ Test fuel pressure (if possible)
│     └─ Replace HPFP
│
├─ No P0087 but hard start?
│  └─ Test fuel pressure
│     ├─ Low pressure → HPFP
│     └─ Good pressure → Other issue
│
└─ Won't start at all?
   ├─ Check low pressure system first
   └─ If low pressure OK → HPFP
```

---

## Repair Options

### Option 1: Replace HPFP Only
**Cost:** $600-1,200 (parts + labor)
**Labor:** 2-3 hours
**Parts:** HPFP only

**When to choose:**
- Confirmed HPFP failure
- No metal shavings in fuel system

---

### Option 2: HPFP + Clean Fuel System
**Cost:** $800-1,500
**Additional work:**
- Clean fuel rail
- Inspect/replace injectors if contaminated
- Flush high pressure lines

**When to choose:**
- Metal shavings found
- Multiple previous HPFP failures
- Injector codes present

---

## Parts Information

### OEM HPFP:
**Part Number:** 13517588879 (Bosch)
**Cost:** $400-600

### Aftermarket:
**Brands:** Bosch, Hitachi
**Cost:** $200-400

**Note:** Use OEM or quality aftermarket only
- Cheap pumps fail quickly
- Can contaminate fuel system

---

## Root Causes of HPFP Failure

### Primary Causes:
1. **Poor fuel quality**
   - Low octane fuel
   - Contaminated fuel
   - Water in fuel

2. **Mechanical wear**
   - High mileage (80k+)
   - Cam lobe wear
   - Internal pump wear

3. **Manufacturing defect**
   - Early N14 pumps had issues
   - Improved design in later pumps

### Prevention:
- Use 91+ octane fuel (required for turbo)
- Fill at reputable stations
- Replace fuel filter regularly
- Don't run fuel tank below 1/4

---

## Common Misdiagnosis

### Symptoms that LOOK like HPFP but aren't:

**Low pressure fuel pump failure:**
- Similar symptoms
- Check low pressure first

**Ignition system failure:**
- Also causes hard start
- But usually shows misfire codes

**Cam position sensor:**
- Can cause no-start
- Different code pattern

**Carbon buildup:**
- Rough idle, hesitation
- But starts normally

---

## After Replacement

### Break-in:
- First 160 km: drive gently
- Avoid full throttle
- Monitor starting behavior

### Verify Fix:
- Starting should be normal (1-2 sec crank)
- No P0087 codes
- Smooth acceleration

### Prevention:
- Use quality fuel
- Don't run tank low
- Monitor long-term fuel trims with scan tool

---

## Related Issues Often Found With HPFP

**Injectors:**
- If HPFP failed catastrophically
- Metal shavings can damage injectors
- Symptoms: Misfires, rough idle

**Fuel Pressure Sensor:**
- Can give false readings
- Leads to misdiagnosis

**Low Pressure Pump:**
- Weak pump stresses HPFP
- Replace both if low pressure pump is weak

---

## DIY vs Professional

### DIY (Possible but challenging):
**Pros:**
- Save labor cost
- Not extremely difficult

**Cons:**
- Need special socket (27mm thin wall)
- Fuel system depressurization required
- Safety hazard (high pressure fuel)
- Timing/alignment critical

**Skill Level:** Intermediate to Advanced

---

### Professional (Recommended):
**Pros:**
- Proper tools and experience
- Warranty on work
- Faster completion

**Cost:** $600-1,200 total

---

## Summary Checklist

**Suspect HPFP if:**
- ✓ P0087 code present
- ✓ Hard starting (long crank)
- ✓ Won't rev past 2-3k RPM
- ✓ Intermittent loss of power
- ✓ Low fuel pressure reading

**Before replacing:**
- ✓ Scan for codes
- ✓ Test low pressure system
- ✓ Verify fuel pressure at rail
- ✓ Check fuel quality

**Replacement:**
- ✓ Use OEM or quality parts
- ✓ Consider fuel system cleaning
- ✓ Test immediately after install
- ✓ Monitor for recurrence

---

## Related Documentation
- [Fuel System Components](../fuel-system/fuel-components.md)
- [No Start Diagnosis](no-start.md)
- [Engine Components](../engine/N14-engine-components.md)

---

## 🔗 Related Guides

**If you're experiencing HPFP issues:**

1. [HPFP Component Guide](../engine/components/fuel-injection/01-HPFP.md) - Detailed failure modes, testing, replacement guide
2. [No Start Diagnosis](no-start.md) - Won't start troubleshooting
3. [Fuel Pressure Testing](fuel-pressure-test.md) - How to test fuel pressure
