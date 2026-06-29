<div align="center">
# FARHAN HUSSAIN
 
**B.Tech CSE — Artificial Intelligence & Machine Learning**
K.R. Mangalam University
 
`Engineering data pipelines — not decorating dashboards.`
 
<br/>
![Python](https://img.shields.io/badge/PYTHON-000000?style=for-the-badge&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/BASH-000000?style=for-the-badge&logo=gnubash&logoColor=white)
![Linux](https://img.shields.io/badge/LINUX-000000?style=for-the-badge&logo=linux&logoColor=white)
![NixOS](https://img.shields.io/badge/NIXOS-000000?style=for-the-badge&logo=nixos&logoColor=white)
![Pandas](https://img.shields.io/badge/PANDAS-000000?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NUMPY-000000?style=for-the-badge&logo=numpy&logoColor=white)
![Git](https://img.shields.io/badge/GIT-000000?style=for-the-badge&logo=git&logoColor=white)
 
</div>
<br/>
```
┌─[ profile.status ]───────────────────────────────────────────────┐
│ user      : farhan.hussain                                       │
│ program   : b.tech cse — artificial intelligence & ml            │
│ institute : k.r. mangalam university                             │
│ roll_no   : 2501730002                                           │
│                                                                  │
│ ideology  : pipelines > pixels  //  logic > layout               │
│ status    : ACTIVE — compiling knowledge, shipping code          │
└──────────────────────────────────────────────────────────────────┘
```
 
```
┌─[ workstation.mode ]─────────────────────────────────────────────┐
│ distro.a  : nixos — declarative, reproducible builds             │
│ distro.b  : elementary os — pantheon desktop env                 │
│ shell     : bash                                                 │
│ toolchain : python3 · pip · venv · git                           │
│                                                                  │
│ workflow  : terminal-first, gui-optional                         │
│ frontend  : academic / exam-scope only — not a focus area        │
└──────────────────────────────────────────────────────────────────┘
```
 
```
# core.ideology
# pipeline-first · oop-clean · automation-by-default · frontend = academic-only
```
 
<br/>
## `$ cat language_distribution.log`
 
```
LANGUAGE DISTRIBUTION
──────────────────────────────────────────────────
Python            85%  █████████████████░░░
Bash / Shell      10%  ██░░░░░░░░░░░░░░░░░░
HTML / CSS / JS    5%  █░░░░░░░░░░░░░░░░░░░
──────────────────────────────────────────────────
> primary_language : python
> frontend_scope   : academic / exam-only
```
 
<br/>
## `$ ls -la ./projects/`
 
### 01 // Campus Energy Analytics Dashboard
 
`capstone project` — OOP-driven ingestion-to-insight pipeline for multi-building energy telemetry.
 
**Engineering surface:**
- Fault-tolerant multi-source ingestion (`on_bad_lines='skip'`) — malformed rows are quarantined, never silently dropped.
- Anomaly-aware cleaning pass executed before any aggregation touches the frame.
- Temporal normalization via `resample('D')` for consistent daily-frequency analysis.
- Multi-level logging (`INFO` / `WARNING` / `ERROR`) instrumented through the pipeline, not bolted on after the fact.
- Multi-panel Matplotlib rendering generated programmatically from validated output only.
```bash
$ python3 energy_pipeline.py --batch ./logs/raw/
 
[14:02:01] INIT      :: bootstrapping OOP pipeline objects
[14:02:01] INGEST    :: scanning raw building logs (sources=14)
[14:02:02] PARSE     :: on_bad_lines='skip' -> malformed rows quarantined (37)
[14:02:02] VALIDATE  :: schema check passed -> 9/9 required columns present
[14:02:03] CLEAN     :: anomaly filter applied -> outliers clipped (z > 3.0)
[14:02:03] TRANSFORM :: resample('D') -> daily-frequency normalization complete
[14:02:04] LOG       :: multi-level logger attached [INFO|WARNING|ERROR]
[14:02:05] RENDER    :: matplotlib multi-panel canvas -> 4 subplots generated
[14:02:05] EXIT      :: pipeline terminated -> status 0, runtime 4.21s
```
 
**Source:** [`/ASSIGNMENT-5-CAPSTONE-PROJECT`](https://github.com/farhan0386/assignments/tree/main/SEM-1/PYTHON/ASSIGNMENT-5-CAPSTONE-PROJECT)
 
---
 
### 02 // Automated Weather Data Analytics Engine
 
`data-repair engine` — built for sensor environments where missing or corrupted readings are the default, not the exception.
 
**Engineering surface:**
- Time-based linear interpolation (`interpolate(method='linear')`) restores missing segments without distorting trend shape.
- Deprecation-safe aggregation using the `'ME'` month-end frequency alias in place of legacy offsets.
- Dual-axis (`twinx()`) visualization to compare temperature and humidity on independent scales without misleading overlap.
```bash
$ python3 weather_analysis.py --repair --visualize
 
[09:14:11] MOUNT     :: sensor stream mounted -> corrupted segments detected
[09:14:11] REPAIR    :: interpolate(method='linear') -> 142 NaN cells restored
[09:14:12] AGGREGATE :: resample(freq='ME') -> month-end, non-deprecated alias
[09:14:12] CHECK     :: dtype integrity verified -> no silent coercion
[09:14:13] PLOT      :: twinx() -> dual-axis (temp C / humidity %) rendered
[09:14:13] EXIT      :: pipeline terminated -> status 0, runtime 2.04s
```
 
**Source:** [`/ASSIGNMENT-4/weather_analysis.py`](https://github.com/farhan0386/assignments/blob/main/SEM-1/PYTHON/ASSIGNMENT-4/weather_analysis.py)
 
---
 
### 03 // Algorithmic Practice Sandbox
 
`daily infrastructure` — running log of core data-structure, algorithm, and shell-automation implementations.
 
**Engineering surface:**
- Hand-rolled Stacks, Linked Lists, and 2D matrix traversal routines — no abstraction shortcuts taken.
- Custom sorting implementations validated for complexity, not just output correctness.
- Bash/Shell performance-monitoring modules for lightweight, dependency-free system introspection.
```bash
$ ./run_suite.sh --all
 
[DS  ] stack.push_pop() .......... PASS
[DS  ] linked_list.traverse() .... PASS
[DS  ] matrix.transpose(4x4) ..... PASS  (dimensions verified)
[ALGO] custom_sort(n=10000) ...... PASS  (O(n log n) confirmed)
[SH  ] perf_monitor.sh ........... PASS  (cpu/mem sampled @1s)
 
ALL CHECKS GREEN -- 5/5 modules, 0 failures
```
 
**Source:** [`/btech-codebase`](https://github.com/farhan0386/btech-codebase)
 
---
 
<div align="center">
```
$ echo $STATUS
"compiling. shipping. iterating."
```
 
<sub>pipeline-first, always.</sub>
 
</div>
 