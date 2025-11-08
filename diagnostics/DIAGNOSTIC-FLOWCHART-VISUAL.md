# N14 Visual Diagnostic Flowcharts
## Interactive Diagrams for Quick Problem Diagnosis

---

## 🚨 Critical Symptoms Flowchart

```mermaid
flowchart TD
    Start([Engine Problem?]) --> Noise{Noise Type?}
    Start --> Performance{Performance Issue?}
    Start --> Leak{Fluid Leak?}

    Noise -->|Death Rattle<br/>Cold Start| TimingChain[⚠️ TIMING CHAIN<br/>CRITICAL]
    Noise -->|Hissing after<br/>4000 RPM| BoostLeak[⚠️ BOOST LEAK<br/>URGENT]
    Noise -->|Grinding/Whining| VacuumPump[Vacuum Pump<br/>or Turbo]

    Performance -->|Won't Start<br/>Cranks OK| FuelIssue{Fuel or Spark?}
    Performance -->|Loss of Power<br/>Under Boost| TurboIssue[Turbo/Boost<br/>System]
    Performance -->|Rough Idle<br/>Hesitation| CarbonBuild[Carbon Buildup<br/>or Misfires]

    Leak -->|Coolant<br/>Left Side| Thermostat[Thermostat<br/>Housing]
    Leak -->|Oil<br/>Top of Engine| ValveCover[Valve Cover<br/>Gasket]
    Leak -->|Oil<br/>Low Pressure| OilPump[Oil Pump<br/>or Seals]

    FuelIssue -->|No Fuel Pressure| HPFP[High Pressure<br/>Fuel Pump]
    FuelIssue -->|Has Fuel Pressure| Ignition[Spark Plugs<br/>Ignition Coils]

    TimingChain -->|Action| TC_Action[Replace Timing<br/>Chain Kit<br/>R12-25k]
    BoostLeak -->|Action| BL_Action[Find Leak<br/>Replace Hoses<br/>R1-5k]
    HPFP -->|Action| HPFP_Action[Replace HPFP<br/>R6-12k]
    CarbonBuild -->|Action| Carbon_Action[Walnut Blasting<br/>R3-6k]
    ValveCover -->|Action| VC_Action[Replace Gasket<br/>R1-3k]

    style TimingChain fill:#ff6b6b,stroke:#c92a2a,color:#fff
    style BoostLeak fill:#ff6b6b,stroke:#c92a2a,color:#fff
    style HPFP fill:#ffd43b,stroke:#fab005
    style CarbonBuild fill:#ffd43b,stroke:#fab005
    style Thermostat fill:#74c0fc,stroke:#1c7ed6
    style ValveCover fill:#74c0fc,stroke:#1c7ed6
```

---

## 🔧 Timing Chain Decision Tree

```mermaid
flowchart TD
    Start([Cold Start Engine]) --> Listen{Hear Rattling?}

    Listen -->|No Rattle| Good[✅ Timing Chain OK<br/>Continue Monitoring]
    Listen -->|Yes, Rattling| Duration{How Long?}

    Duration -->|1-2 seconds| Early[⚠️ EARLY WARNING<br/>Stage 1]
    Duration -->|2-5 seconds| Moderate[⚠️ MODERATE<br/>Stage 2]
    Duration -->|Continuous| Severe[🚨 SEVERE<br/>Stage 3]

    Early --> Early_Action[Plan Replacement<br/>Within 10,000 km<br/>Not Urgent Yet]
    Moderate --> Mod_Action[Schedule Repair<br/>Within 5,000 km<br/>URGENT]
    Severe --> Sev_Action[STOP DRIVING<br/>Repair Immediately<br/>Engine at Risk]

    Early_Action --> Cost[Cost: R12,000-25,000]
    Mod_Action --> Cost
    Sev_Action --> Risk[Risk: R40,000-100,000<br/>if chain jumps]

    Good --> Monitor{2007-2009<br/>Model?}
    Monitor -->|Yes| Preventive[Consider Preventive<br/>Replacement at<br/>80,000 km]
    Monitor -->|No| Continue[Continue Normal<br/>Maintenance]

    style Severe fill:#ff6b6b,stroke:#c92a2a,color:#fff
    style Moderate fill:#ffd43b,stroke:#fab005
    style Early fill:#74c0fc,stroke:#1c7ed6
    style Good fill:#51cf66,stroke:#2f9e44,color:#fff
    style Risk fill:#ff6b6b,stroke:#c92a2a,color:#fff
```

---

## 🔍 Oil Pressure Monitoring (Post-Crankshaft Work)

```mermaid
flowchart TD
    Start([Install Mechanical<br/>Oil Pressure Gauge]) --> WarmUp[Warm Engine<br/>to 80-90°C]

    WarmUp --> IdleCheck{Idle Pressure?}

    IdleCheck -->|Below 1.0 bar| Critical[🚨 CRITICAL<br/>Stop Engine]
    IdleCheck -->|1.0-1.5 bar| Marginal[⚠️ MARGINAL<br/>Investigate]
    IdleCheck -->|1.5+ bar| Good_Idle[✅ Good]

    Good_Idle --> RPM_Check{Pressure at<br/>4,000 RPM?}

    RPM_Check -->|Below 3.0 bar| Low_RPM[⚠️ LOW<br/>Check Pump]
    RPM_Check -->|3.0-4.0 bar| OK_RPM[Acceptable<br/>Monitor Closely]
    RPM_Check -->|4.0+ bar| Excellent[✅ EXCELLENT<br/>Perfect]

    Critical --> Action1[1. Check Oil Level<br/>2. Inspect for Leaks<br/>3. TOW to Shop]
    Marginal --> Action2[1. Monitor Daily<br/>2. Check Pickup Screen<br/>3. Consider Pump Upgrade]
    Low_RPM --> Action3[Consider Oil Pump<br/>Upgrade<br/>R13-26k]

    Excellent --> Schedule[Continue<br/>Break-in Schedule:<br/>• 500 km oil change<br/>• 1,500 km oil change<br/>• 3,000 km oil change]

    style Critical fill:#ff6b6b,stroke:#c92a2a,color:#fff
    style Marginal fill:#ffd43b,stroke:#fab005
    style Excellent fill:#51cf66,stroke:#2f9e44,color:#fff
    style Good_Idle fill:#51cf66,stroke:#2f9e44,color:#fff
```

---

## 📅 Maintenance Timeline

```mermaid
gantt
    title N14 Maintenance Schedule (Kilometers)
    dateFormat X
    axisFormat %s km

    section Critical
    Oil Changes (Every 8k)           :crit, 0, 8000
    Oil Changes (Every 8k)           :crit, 8000, 16000
    Oil Changes (Every 8k)           :crit, 16000, 24000
    Oil Changes (Every 8k)           :crit, 24000, 32000
    Oil Changes (Every 8k)           :crit, 32000, 40000
    Oil Changes (Every 8k)           :crit, 40000, 48000

    section Carbon Cleaning
    First Carbon Cleaning            :active, 48000, 64000
    Second Carbon Cleaning           :96000, 112000

    section Major Service
    Spark Plugs                      :96000, 98000
    Timing Chain (if not done)       :done, 80000, 82000
    Vacuum Pump                      :130000, 132000
    Water Pump                       :130000, 132000

    section Preventive
    Bypass Valve Inspect             :50000, 130000
    PCV System Check                 :48000, 96000
```

---

## 🔄 Carbon Buildup Progression

```mermaid
flowchart LR
    Start([New Engine]) -->|0-24k km| Stage1[Light Deposits<br/>No Symptoms]
    Stage1 -->|24-48k km| Stage2[Moderate Buildup<br/>Slight Rough Idle]
    Stage2 -->|48-80k km| Stage3[Severe Buildup<br/>Power Loss]
    Stage3 -->|80k+ km| Stage4[Critical<br/>Misfires/Won't Start]

    Stage2 -.->|Clean Now| Clean1[Walnut Blasting<br/>R3-6k]
    Stage3 -.->|Clean ASAP| Clean2[Walnut Blasting<br/>R3-6k]
    Stage4 -.->|URGENT| Clean3[Walnut Blasting<br/>+ Possible Cat Damage<br/>R8-18k]

    Clean1 --> Prevention[Install Catch Can<br/>R2-4k<br/>Extends to 64k km]
    Clean2 --> Prevention
    Clean3 --> Prevention

    style Stage1 fill:#51cf66,stroke:#2f9e44
    style Stage2 fill:#ffd43b,stroke:#fab005
    style Stage3 fill:#ff922b,stroke:#e8590c
    style Stage4 fill:#ff6b6b,stroke:#c92a2a,color:#fff
    style Clean1 fill:#74c0fc,stroke:#1c7ed6
    style Clean2 fill:#74c0fc,stroke:#1c7ed6
    style Clean3 fill:#74c0fc,stroke:#1c7ed6
```

---

## 🌡️ Overheating Diagnosis Tree

```mermaid
flowchart TD
    Start([Engine Overheating]) --> Coolant{Coolant Level?}

    Coolant -->|Low/Empty| LeakCheck{Visible Leak?}
    Coolant -->|Full| TempCheck{Actual Temp?}

    LeakCheck -->|Yes, Left Side| Thermostat[Thermostat Housing<br/>VERY COMMON<br/>R1.5-3.5k]
    LeakCheck -->|Yes, Bottom| Radiator[Radiator or<br/>Water Pump<br/>R3.5-7k]
    LeakCheck -->|No Visible Leak| Pressure[Pressure Test<br/>Head Gasket?]

    TempCheck -->|Actually Normal| Sensor[Coolant Temp Sensor<br/>False Reading<br/>R400-1,200]
    TempCheck -->|Actually High| Cooling{Fans Running?}

    Cooling -->|Fans Not Running| Fan[Fan Control Module<br/>or Fan Motor<br/>R1.5-3.5k]
    Cooling -->|Fans Running| Flow{Coolant Flowing?}

    Flow -->|No Flow| Pump[Water Pump Failed<br/>R3.5-7k]
    Flow -->|Flowing| Blocked[Thermostat Stuck<br/>or Radiator Blocked<br/>R1.5-5k]

    Pressure -->|White Smoke| HG[Head Gasket Failure<br/>EXPENSIVE<br/>R15-30k]

    style Thermostat fill:#ffd43b,stroke:#fab005
    style HG fill:#ff6b6b,stroke:#c92a2a,color:#fff
    style Sensor fill:#51cf66,stroke:#2f9e44
```

---

## 💨 Boost System Diagnosis

```mermaid
flowchart TD
    Start([Low Boost/Power Loss]) --> Code{Check OBD Codes}

    Code -->|P0234 Overboost| Wastegate[Wastegate Stuck<br/>or N75 Valve<br/>R1.5-4k]
    Code -->|P0299 Underboost| Leak{Boost Leak?}
    Code -->|No Codes| Manual[Manual Testing<br/>Required]

    Leak -->|Hissing Sound| FindLeak[Smoke Test<br/>or Soapy Water<br/>R500-1.5k]
    Leak -->|No Sound| Bypass[Bypass Valve<br/>Failed<br/>R1.2-2.5k]

    FindLeak --> Common{Location?}
    Common -->|Intercooler Hoses| Hoses[Replace Hoses<br/>Common Failure<br/>R800-2k]
    Common -->|Intercooler Itself| IC[Replace Intercooler<br/>R3-6k]
    Common -->|Turbo Outlet| Turbo[Check Turbo<br/>Compressor Wheel]

    Manual --> Pressure[Install Boost Gauge<br/>Monitor Actual PSI]
    Pressure --> Target{Reaches<br/>1.2 bar?}

    Target -->|No| Turbo_Issue[Turbo Problem<br/>or Wastegate<br/>R8-15k]
    Target -->|Yes but Drops| Bypass

    style Hoses fill:#74c0fc,stroke:#1c7ed6
    style Bypass fill:#ffd43b,stroke:#fab005
    style Turbo_Issue fill:#ff6b6b,stroke:#c92a2a,color:#fff
```

---

## 🔩 Component Relationship Diagram

```mermaid
graph TB
    subgraph Critical_Chain[Critical Timing Chain System]
        Crank[Crankshaft] -->|Drives| Chain[Timing Chain]
        Chain -->|Drives| IntakeCam[Intake Camshaft]
        Chain -->|Drives| ExhaustCam[Exhaust Camshaft]
        Tensioner[Hydraulic Tensioner] -.->|Tensions| Chain
        OilPump[Oil Pump] -.->|Pressure to| Tensioner

        IntakeCam -->|Drives| VacuumPump[⚠️ Vacuum Pump<br/>Failure Risk]
        IntakeCam -->|Opens| IntakeValves[Intake Valves]
        ExhaustCam -->|Opens| ExhaustValves[Exhaust Valves]
    end

    subgraph Fuel_System[High Pressure Fuel System]
        Tank[Fuel Tank] -->|4 bar| LowPump[Low Pressure Pump]
        LowPump -->|Supplies| HPFP[High Pressure<br/>Fuel Pump]
        IntakeCam -.->|Drives| HPFP
        HPFP -->|100-200 bar| Rail[Fuel Rail]
        Rail --> Injectors[Direct Injectors]
    end

    subgraph Turbo_System[Turbocharger System]
        Turbo[Turbocharger] -->|Compressed Air| Intercooler[Intercooler]
        Intercooler -->|Cooled Air| Throttle[Throttle Body]
        Throttle --> Intake[Intake Manifold]
        Intake -.->|No Fuel on Valves| IntakeValves
        IntakeValves -.->|Carbon Builds Up| Carbon[⚠️ Carbon Deposits]
    end

    style Chain fill:#ff6b6b,stroke:#c92a2a,color:#fff
    style Tensioner fill:#ff6b6b,stroke:#c92a2a,color:#fff
    style VacuumPump fill:#ffd43b,stroke:#fab005
    style HPFP fill:#ffd43b,stroke:#fab005
    style Carbon fill:#ffd43b,stroke:#fab005
```

---

## 🛠️ Post-Major-Repair Checklist

```mermaid
stateDiagram-v2
    [*] --> Install_Gauge: Install Mechanical<br/>Oil Pressure Gauge

    Install_Gauge --> First_500km: First 500 km

    state First_500km {
        [*] --> Monitor_Daily: Check Pressure Daily
        Monitor_Daily --> Check_Level: Check Oil Level<br/>Every 100 km
        Check_Level --> Listen: Listen for Noises
        Listen --> [*]
    }

    First_500km --> Oil_Change_1: Oil Change at 500 km
    Oil_Change_1 --> Next_1000km: 500-1,500 km

    state Next_1000km {
        [*] --> Monitor_Weekly: Check Pressure Weekly
        Monitor_Weekly --> Check_Level_2: Check Oil Level<br/>Every 300 km
        Check_Level_2 --> [*]
    }

    Next_1000km --> Oil_Change_2: Oil Change at 1,500 km
    Oil_Change_2 --> Next_1500km: 1,500-3,000 km

    state Next_1500km {
        [*] --> Stable: Pressure Should<br/>Be Stable Now
        Stable --> [*]
    }

    Next_1500km --> Oil_Change_3: Oil Change at 3,000 km
    Oil_Change_3 --> Normal: Normal Service<br/>Every 8,000 km
    Normal --> [*]
```

---

## 💡 How to Use These Diagrams

1. **Navigate by symptom** - Start with the relevant flowchart
2. **Follow the decision tree** - Answer questions to narrow down the problem
3. **Check costs** - Repair costs shown in South African Rand
4. **Refer to detailed guides** - Links provided throughout documentation

**All diagrams are interactive on GitHub and mobile-friendly!**

---

## 📱 Mobile Viewing

These Mermaid diagrams render perfectly on:
- ✅ GitHub website (desktop and mobile)
- ✅ GitHub mobile app
- ✅ GitHub Pages
- ✅ Any modern browser

**Tip:** On mobile, diagrams can be zoomed and panned for easy viewing.
