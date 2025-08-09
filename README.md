# MES Simulation – AnyLogic 8.9.5 Personal Learning Edition

- This project is a simplified Manufacturing Execution System (MES) simulation built in AnyLogic 8.9.5 PLE. It demonstrates how jobs flow through a manufacturing process with production, quality control, and warehouse update stages, using Service blocks and ResourcePools.
- Built to practice MES concepts using AnyLogic's discrete event simulation capabilities.

## Project Structure

```
MES_Simulation/
├── MES_Simulation.alp
├── README.md
├── screenshots
```

## Setup

### 1. Open in AnyLogic

- Launch AnyLogic 8.9.5 PLE
- Go to File -> Open Model
- Select MES_Simulation.alp

### 2. Run Simulation

### 3. Watch the Flow

- Jobs move from jobSource -> processJob -> qualityCheck -> updateInventory -> jobSink
- ResourcePools control capacity for each stage

### 4. View Live Data

- Open jobsInSystemPlot to see how many jobs are at each stage over time

## Time Plot Variables

The jobsInSystemPlot displays:
- processJob.size() -> Number of jobs in production
- qualityCheck.size() -> Number of jobs in quality inspection
- updateInventory.size() -> Number of jobs in inventory update

## Example Output

### Run-View, Process-flow and Timeplot
![run-view-diagram](https://github.com/vbx14/mini-mes/blob/b500d2ed0b5606ff879062ac8ab976059d35546d/screenshots/HTML%20UI%20for%20API%20Test.png)

##  Installation Notes

- Built for AnyLogic 8.9.5 Personal Learning Edition
- No external dependencies needed
- ResourcePools are directly linked to their respective Service blocks