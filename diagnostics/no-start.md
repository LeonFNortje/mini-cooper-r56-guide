# No Start Diagnosis - Complete Guide

## Overview

When your Mini Cooper S R56 won't start, there are several possible causes. This guide helps you systematically diagnose the issue.

---

## Initial Assessment

### First, Identify the Type of No-Start:

**Type 1: No Crank**
- Turn key, nothing happens
- No sound at all
- Or: Clicking sound but engine doesn't turn over

**Type 2: Cranks But Won't Fire**
- Engine turns over normally
- But never catches and runs

**Type 3: Starts Then Immediately Dies**
- Fires for 1-2 seconds
- Then stalls

**Type 4: Won't Start After Specific Event**
- After boost leak / turbo issue
- After overheating
- After running out of fuel
- After stalling

---

## Type 1: No Crank (Won't Turn Over)

### Symptoms:
- ✓ Turn key to START position
- ✓ Dash lights come on
- ✓ But engine doesn't crank (or just clicks)

### Common Causes:

#### 1. Dead Battery (60%)

**Symptoms:**
- Dash lights dim or don't come on
- Clicking sound from starter
- Interior lights dim when trying to start
- Accessories weak or don't work

**Quick Test:**
1. Turn on headlights
2. Try to start
3. Headlights go very dim = dead battery

**Confirmation:**
- Use multimeter
- Battery should be 12.4V+ when off
- 11-12V = low/dying battery
- Below 11V = dead battery

**Solutions:**
- Jump start
- Charge battery
- Replace battery if old (3-5 years typical life)

**Battery Location:** Trunk/boot area

**Cost:**
- Jump start: Free
- New battery: $100-200

---

#### 2. Starter Motor Failure (25%)

**Symptoms:**
- Clicking sound from engine bay
- Battery is good (tested at 12.4V+)
- All dash lights bright
- Just won't crank

**Quick Test:**
1. Turn on headlights (keep on)
2. Try to start
3. Headlights stay bright BUT clicking sound = starter issue
4. Headlights dim = battery issue

**Confirmation:**
- Have someone tap starter with hammer while you try to start
- If it starts: Starter is failing

**Starter Location:** Bottom of engine, transmission area

**Solutions:**
- Replace starter motor
- Parts: $150-300
- Labor: 2-3 hours

**Cost:** $300-600 total

---

#### 3. Ignition Switch Failure (10%)

**Symptoms:**
- Turn key, nothing happens
- Dash may or may not light up
- Intermittent (works sometimes)

**Quick Test:**
1. Try starting in different positions:
   - Turn wheel left/right
   - Wiggle key while turning
   - Push/pull key while turning

**If it starts with wiggling:** Ignition switch or cylinder issue

**Solutions:**
- Replace ignition switch: $100-200
- Or replace ignition cylinder: $150-300

**Cost:** $200-500

---

#### 4. Neutral Safety Switch (Automatic Only) (3%)

**Symptoms:**
- Won't start in PARK
- Might start in NEUTRAL

**Quick Test:**
1. Try starting in PARK (normal position)
2. If doesn't work, try NEUTRAL
3. If starts in NEUTRAL: Neutral safety switch issue

**Solutions:**
- Adjust switch: $50-100
- Replace switch: $100-200

---

#### 5. Clutch Safety Switch (Manual Only) (2%)

**Symptoms:**
- Won't start even with clutch pedal down
- Worked fine before

**Quick Test:**
1. Press clutch fully
2. Have someone watch clutch switch at pedal
3. Should click when pressed

**Solutions:**
- Adjust switch: $50
- Replace switch: $50-100

---

### No-Crank Diagnostic Flowchart:

```
WON'T CRANK?
│
├─ Battery voltage?
│  ├─ Below 12V → Charge or replace battery
│  └─ Above 12.4V → Continue
│
├─ Headlight test during crank attempt:
│  ├─ Lights dim significantly → Battery weak despite voltage
│  ├─ Lights stay bright + clicking → Starter motor
│  └─ Lights stay bright + no sound → Ignition switch or safety switch
│
├─ For clicking sound:
│  └─ Tap starter while cranking → If starts, replace starter
│
└─ For no sound at all:
   ├─ Wiggle key while turning → If works, ignition switch
   ├─ Try neutral (auto) → If works, neutral safety switch
   └─ Check clutch switch (manual) → May need adjustment
```

---

## Type 2: Cranks But Won't Fire

### Symptoms:
- ✓ Engine turns over normally
- ✓ Good cranking speed
- ✓ But never fires and runs

### This Indicates:
Either **no fuel** or **no spark**

---

### Determining: Fuel or Spark?

**Quick Test:**
1. Try to start engine
2. Smell exhaust pipe immediately after
3. **Strong fuel smell** = Getting fuel, likely spark issue
4. **No fuel smell** = Not getting fuel

---

### Path A: No Fuel

#### Common Causes:

**1. High Pressure Fuel Pump (HPFP) Failure (50%)**

**Symptoms:**
- Hard starting before complete failure
- Long crank times
- P0087 code (if scanned previously)
- May have worked intermittently

**Quick Test:**
1. Turn key to ON (don't start)
2. Listen at fuel tank for pump hum (2 seconds)
3. If no hum: Low pressure pump failed
4. If hum present: HPFP likely failed

**Detailed Diagnosis:**
- See: [HPFP Diagnosis Guide](HPFP-diagnosis.md)

**Solutions:**
- Replace HPFP
- Cost: $600-1,200

---

**2. Low Pressure Fuel Pump Failure (20%)**

**Symptoms:**
- Similar to HPFP but less common
- No fuel pump sound when key turned ON

**Quick Test:**
1. Turn key to ON
2. Listen at fuel tank (put ear near fuel door)
3. Should hear 2-second hum
4. No hum = pump failed

**Solutions:**
- Replace in-tank fuel pump
- Cost: $300-600

---

**3. Fuel Relay / Fuse (15%)**

**Symptoms:**
- No fuel pump sound
- Sudden failure (worked fine, now doesn't)

**Quick Test:**
1. Check fuel pump fuse (under hood or in trunk)
2. Check fuel pump relay
3. Swap relay with another similar relay (test)

**Solutions:**
- Replace fuse: $1
- Replace relay: $10-30

---

**4. Empty Fuel Tank (10%)**

**Symptoms:**
- Fuel gauge shows empty (or very low)
- Ran out of fuel

**Issues:**
- Fuel gauge may be inaccurate
- May show 1/8 tank but actually empty
- After running dry, system needs priming

**Solutions:**
- Add fuel (5+ gallons)
- May need multiple crank attempts (10 seconds on, 30 seconds off)
- May need to prime fuel system

**After Refueling:**
1. Turn key ON (don't start), wait 5 seconds, OFF
2. Repeat 5 times
3. Then try starting

---

**5. Clogged Fuel Filter (5%)**

**Symptoms:**
- Progressive difficulty starting
- Eventually won't start

**Solutions:**
- Replace fuel filter
- Cost: $50-150

---

### Path B: No Spark

#### Common Causes:

**1. Crankshaft Position Sensor Failure (40%)**

**Symptoms:**
- Cranks normally but no fire
- No tach movement while cranking
- P0335 code (crank sensor)

**Quick Test:**
- Watch tachometer while cranking
- Should move slightly
- No movement = likely crank sensor

**Solutions:**
- Replace crank position sensor
- Cost: $100-250

---

**2. Camshaft Position Sensor Failure (30%)**

**Symptoms:**
- Cranks but no start
- P0340 / P0345 codes
- Intermittent before complete failure

**Solutions:**
- Replace cam sensor(s)
- Cost: $150-300 (both sensors)

---

**3. Ignition Coil Failure (Multiple) (15%)**

**Symptoms:**
- Would normally cause misfire, not complete no-start
- Unless multiple coils failed

**Quick Test:**
- Pull spark plugs
- Check for spark (use spark tester)

**Solutions:**
- Replace all 4 coils (if multiple failed)
- Cost: $200-400

---

**4. ECU Failure (10%)**

**Symptoms:**
- Rare but possible
- No codes
- No communication with scanner
- May have gotten wet

**Solutions:**
- ECU repair or replacement
- Cost: $500-1,500

---

**5. Timing Chain Failure (5%)**

**Symptoms:**
- **Death rattle before failure**
- Cranks but timing is wrong
- Won't fire
- Internal engine damage

**Confirmation:**
- Compression test shows no/low compression
- Timing chain broke

**Solutions:**
- Timing chain replacement minimum
- Possible engine rebuild if valves hit pistons
- Cost: $1,500-$8,000+

**See:** [Timing Chain Diagnosis](timing-chain-diagnosis.md)

---

### Cranks But Won't Fire Flowchart:

```
CRANKS BUT WON'T START?
│
├─ Smell fuel at exhaust after cranking?
│  │
│  ├─ YES (strong fuel smell) → SPARK ISSUE
│  │  ├─ Check for spark at plugs
│  │  ├─ Check crank/cam position sensors
│  │  ├─ Check coils
│  │  └─ Scan for codes (P0335, P0340, P0345)
│  │
│  └─ NO (no fuel smell) → FUEL ISSUE
│     ├─ Turn key ON, listen for pump hum
│     │  ├─ No hum → Check fuse/relay, then low pressure pump
│     │  └─ Hum present → HPFP likely failed (P0087 code)
│     ├─ Check fuel level (actually put fuel in)
│     └─ Scan for fuel codes (P0087, P0088)
│
└─ Compression test (if above checks pass)
   └─ Low/no compression → Timing chain or internal damage
```

---

## Type 3: Starts Then Immediately Dies

### Symptoms:
- ✓ Engine fires for 1-3 seconds
- ✓ Then stalls/dies
- ✓ Won't stay running

### Common Causes:

**1. Immobilizer/Security System (40%)**

**Symptoms:**
- Starts briefly then cuts
- Security light flashing
- Key may need reprogramming

**Solutions:**
- Try spare key
- Have key reprogrammed
- Check for aftermarket alarm interference

**Cost:** $50-200

---

**2. MAF Sensor Failure (30%)**

**Symptoms:**
- Starts then dies
- Or runs very rough then stalls
- P0101 code

**Quick Test:**
1. Unplug MAF sensor
2. Try starting
3. If runs (poorly): MAF is bad

**Solutions:**
- Clean MAF sensor (try first)
- Replace MAF sensor
- Cost: $100-300

---

**3. Severe Boost Leak (15%)**

**Symptoms:**
- Starts then stalls
- Major hissing sound
- After turbo problem

**See:** [Boost Leak No-Start](boost-leak-no-start-diagnosis.md)

**Solutions:**
- Find and fix boost leak
- Cost: Varies

---

**4. Throttle Body Issues (10%)**

**Symptoms:**
- Starts then dies at idle
- P2135 throttle position codes

**Solutions:**
- Clean throttle body
- Reset throttle adaptation
- Replace throttle body (rare)

**Cost:** $50-500

---

**5. HPFP Weak (5%)**

**Symptoms:**
- Starts for 2-3 seconds on residual fuel pressure
- Then dies as pump can't maintain pressure

**Solutions:**
- Replace HPFP

**Cost:** $600-1,200

---

## Type 4: Won't Start After Specific Event

### After Boost Leak / Turbo Problem

**Why:**
- ECU in protection mode
- Limp mode preventing start
- Severe boost leak confusing sensors

**Solutions:**
1. Fix boost leak
2. Clear codes
3. Disconnect battery 10 minutes (reset ECU)
4. Try starting

**See:** [Boost Leak No-Start Guide](boost-leak-no-start-diagnosis.md)

---

### After Overheating

**Why:**
- ECU protection engaged
- Coolant temp sensor reading too high
- Possible head gasket failure

**Check:**
- Oil on dipstick (milky = coolant in oil)
- Coolant in expansion tank
- Oil level (too high = coolant in oil)

**Solutions:**
1. Let engine cool completely (1+ hour)
2. Check coolant level
3. Try starting
4. If won't start: May have internal damage

---

### After Running Out of Fuel

**Why:**
- Fuel system needs priming
- Air in high pressure system

**Solutions:**
1. Add at least 5 gallons fuel
2. Turn key ON-OFF 5 times (don't crank)
3. Try starting (may take extended cranking)
4. Let crank 10 seconds, rest 30 seconds, repeat

---

### After Stalling

**Why depends on why it stalled:**

**If stalled during driving:**
- Fuel pump failure
- Ignition failure
- Timing chain failure

**If stalled at idle:**
- Idle control issue
- Throttle body
- MAF sensor

**Diagnosis:** Treat as "Cranks But Won't Fire" above

---

## Emergency Starting Procedures

### Try These if Stuck Somewhere:

**1. Battery Weak:**
- Jump start from another car
- Push start (manual transmission only)

**2. Starter Issue:**
- Tap starter with hammer/tool while trying to start
- Rock car in gear (manual, try to free starter)

**3. Fuel System Issue:**
- Add fuel if low
- Pump prime procedure (key ON-OFF multiple times)

**4. Sensor Issue:**
- Unplug MAF sensor, try starting
- Let engine cool if overheated

**5. Immobilizer:**
- Try spare key
- Lock/unlock car with remote
- Wait 10 minutes, try again

---

## Diagnostic Tools Needed

### Basic:
- Multimeter (battery voltage)
- OBD-II scanner (codes)
- Flashlight

### Advanced:
- Spark tester
- Fuel pressure gauge
- Compression tester
- Scan tool with live data

---

## When to Call for Tow

**Call for tow if:**
- Won't crank and jump start doesn't help
- Cranks but multiple attempts fail
- Unusual noises (grinding, rattling)
- Visible damage or leaks
- Smoke from engine
- Recently overheated
- Recent boost/turbo problem

**May attempt restart if:**
- Seems like battery issue and you have jumper cables
- Just ran out of fuel
- Single isolated incident
- No warning signs before

---

## Preventative Maintenance

### To Avoid No-Start Issues:

**Every Oil Change:**
- Check battery terminals (clean if corroded)
- Listen for unusual sounds (timing chain)

**Annually:**
- Battery test (load test)
- Check charging system

**Replace Preventatively:**
- Battery every 4-5 years
- Spark plugs every 60k miles
- Don't ignore check engine lights

**Warning Signs - Address Immediately:**
- Hard starting
- Long crank times
- Rough idle
- Timing chain rattle
- Any turbo/boost issues

---

## Cost Summary

| Cause | DIY Parts | Shop Total |
|-------|-----------|------------|
| Dead battery | $100-200 | $150-250 |
| Battery terminals cleaning | $5 | $50 |
| Starter motor | $150-300 | $300-600 |
| Ignition switch | $100-200 | $250-450 |
| Fuel pump (low pressure) | $150-300 | $400-700 |
| HPFP | $300-600 | $600-1,200 |
| Fuel pump relay/fuse | $10-30 | $50-100 |
| Crank position sensor | $50-100 | $150-300 |
| Cam position sensors | $100-200 | $250-450 |
| Ignition coils (all 4) | $100-200 | $300-500 |
| MAF sensor | $100-250 | $200-400 |

---

## Related Documentation

**Component Details:**
- [Engine Components](../engine/N14-engine-components.md)
- [Electrical Components](../electrical/electrical-components.md)
- [Fuel System](../fuel-system/fuel-components.md)

**Related Diagnostics:**
- [HPFP Diagnosis](HPFP-diagnosis.md)
- [Timing Chain Diagnosis](timing-chain-diagnosis.md)
- [Boost Leak No-Start](boost-leak-no-start-diagnosis.md)
- [MASTER FLOWCHART](MASTER-DIAGNOSTIC-FLOWCHART.md)

---

## Quick Reference Checklist

**If your Mini won't start:**

- [ ] Check battery voltage (12.4V+?)
- [ ] Try spare key (immobilizer?)
- [ ] Listen for fuel pump (2 sec hum when key ON)
- [ ] Smell exhaust for fuel after cranking
- [ ] Scan for codes (if scanner available)
- [ ] Check for obvious leaks or damage
- [ ] Review any recent symptoms (rattle, boost loss, overheating)
- [ ] Decide: DIY diagnose or call for tow

**Most Common No-Start Causes:**
1. Dead/weak battery (35%)
2. HPFP failure (20%)
3. Starter motor (15%)
4. Crank/cam sensors (10%)
5. Fuel pump/relay (8%)
6. Other (12%)

**Key Takeaway:**
Most no-start issues can be diagnosed systematically. Start with the basics (battery, fuel, spark) and work through the checklist. Don't keep trying to start if you hear unusual noises or smell unusual odors.
