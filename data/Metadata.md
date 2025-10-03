# Workout Automation Datasets

To automate your workout planning, we’ve created three structured CSVs that work together:

---

## 1. **exercises.csv**
A curated library of **50 core exercises** across strength, conditioning, and mobility.  

**Key Columns:**  
- `id` – Unique identifier  
- `name` – Exercise name (e.g., Back Squat, Bench Press)  
- `primary_muscle`, `secondary_muscles` – Main target and assisting muscles  
- `movement_pattern` – Squat, Hinge, Push, Pull, Core, etc.  
- `type` – Strength, Power, Conditioning, Mobility  
- `equipment` – Barbell, Dumbbell, Machine, Bodyweight, etc.  
- `level` – Beginner, Intermediate, Advanced  
- `default_sets`, `default_reps`, `default_duration_sec`, `rest_sec`, `tempo` – Suggested training prescriptions  
- `notes` – Technique or coaching cues  

Best for: Building balanced workouts by pulling exercises based on movement patterns.

---

## 2. **templates.csv**
Reusable **program templates** that define the **structure of a session**.  

**Key Columns:**  
- `template_id` – Unique identifier  
- `name` – Template name (e.g., Push Day, Upper/Lower Split)  
- `goal` – Training goal (Strength, Hypertrophy, General Fitness, Conditioning, Mobility)  
- `structure` – Set style (Straight Sets, Circuit, Intervals)  
- `slots` – Movement patterns with counts (e.g., *Squat:1, Hinge:1, Core:1*)  
- `intensity_guidance` – Effort/RIR or rest instructions  
- `notes` – Coaching reminders  

Best for: Assigning a **workout blueprint** before filling it with specific exercises.

---

## 3. **schemes.csv**
Frameworks for **progressive overload** to apply across weeks.  

**Key Columns:**  
- `prog_id` – Unique identifier  
- `name` – Progression style (e.g., Linear, Double Progression, RPE Wave)  
- `weeks` – Duration of the progression cycle  
- `scheme_type` – Method (Reps-Sets, Rep Range, RPE, Time Intervals)  
- `prescription` – Detailed progression rules (e.g., *Week 1: 4x12 @ 65% → Week 4: 5x6 @ 75%*)  
- `notes` – Guidance on resets/deloads  

Best for: Applying **long-term structure** to your training beyond daily templates.

---

✅ Together:  
- **exercises.csv** = the building blocks  
- **templates.csv** = the workout structures  
- **schemes.csv** = the long-term training logic  

