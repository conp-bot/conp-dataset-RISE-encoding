(This README was developed from the template available [here](https://github.com/katielavigne/documentation/wiki/Experiments-README))
# Relational and Item-Specific Encoding (RISE)

# RISE Encoding

##### tags: `offline, english, french`

This is an encoding test. First, participants must answer whether an object shown on the screen is alive or not by pressing 'yes' or 'no'. In the second part, they must answer whether an object can fit inside another one. There are two parts to this experiment: the practice and the trial. The [recognition test](https://gitlab.pavlovia.org/crisp/rise-recognition) sould follow this one.
This experiment was created based on [this paper](https://doi.org/10.1001/jamapsychiatry.2015.0276))

**Publication:** not available

**Experiment DOI:** [10.1001/jamapsychiatry.2015.0276](https://doi.org/10.1001/jamapsychiatry.2015.0276)

**Primary function assessed:** item-specific, relational

**Secondary functions assessed:** 

## Features
- [x] Repeatability
- [x] Multilingual
- [ ] Validated
- [x] Accessibility
- [ ] Cross-platform
- [ ] Cross-device
- [ ] Cross-species

**Alternate Forms:** 

**Languages:** English, French

**Validation:** not available

**Accessibility:** text instructions

**Platforms:** offline

**Devices:** PC 

**Species:** human

## Development
**Software:** PsychoPy 2023.1.3 Builder

**Requirements:** 

## Administration
- Run this task via PsychoPy (download and unzip this repository) or Pavlovia (fork this repository and set the experiment to "running").
- Files will be saved to the local data directory (PsychoPy) or available for download via the Pavlovia dashboard.

## Procedure and Conditions
This test includes 2 practice trials (item-specific, relational), the first 2 practice trials are response-based, and the last 3 are time-based. The practice is followed by 2 trials of 4 blocks each. Block 1 and 3 are item-specific, and Block 2 and 4 are relational.

## Output Files
Output files are named in the following convention: **subjectID_RISE_Enco_date_time**:
- **.csv** files contain experiment information (participant ID, session, date, experiment name, PsychoPy version, framerate).
- **.log** files contain technical information for debugging purposes.
- **.psydat** files contain more detailed information.

## Scoring
You need to look at the output files to see the scoring.

## Additional Features
- Language selection
- Easy to modify trials & add languages through .csv files.

## Note
Please note that PsychoPy delivers millisecond precision, but the measured timings can be affected by different aspects such as monitors, drivers, OS, coding errors, keyboards, etc. More information can be found [here]
(https://www.psychopy.org/general/timing/millisecondPrecision.html).

Also note that, you need to press '5' to start the trial.

## CSV Output Explanations

## Variables Description

| Variable Name                   | Description |
|---------------------------------|-------------|
| `CorrectResponse`               | 1 or 2. |
| `Pairing`                       | I# or A# for Item or Associative block followed by the position of the sitmilus in the trial|
| `SessionTime`                   | The time in HH:mm:ss.SSS format when the RISE experiment started (including practice and instructions). Note: There is a small delay between the time we record the SessionTime and the time the task actually started. `SessionTime.RTTime` allows to correct this delay. |
| `SessionTime.RTTime`            | The time in seconds between we recorded the SessionTime and the RISE experiment actually started. |
| `anyvariablename.started`       | Variable's starting time in seconds since the RISE experiment was started (including practice and instructions). |
| `anyvariablename.stopped`       | Variable's stopping time in seconds since the RISE experiment was started (including practice and instructions). |
| `anyvariablename.rt`            | Variable's rating time in seconds since the routine was started. |
| `anyvariablename.time`          | The time the variable was pressed in seconds since the RISE experiment was started (including practice and instructions). |
| `img.RESP`                      | The answer of the participant (0 for img1 and 1 for img2). |
| `img.CRESP`                     | The correct answer. |
| `img.ACC`                       | 1 if RESP matches CRESP otherwise 0. |
| `img.RT`                        | Time in seconds taken to respond to the trial during the 4-second answer window of the trial's routine. |
| `img.RTTime`                    | Save the time in seconds when the participant answered since the beginning of the experiment. |
| `signal_ctdown.time`            | The different times in seconds when the task received a "5" during the countdown's routine. |
| `img.RTTimeSyncCdown`           | Save the time in seconds when the participant answered since the beginning of the countdown's. |
| `signal.time`                   | The different times in seconds when the task received a "5" during the trial's routine. |
| `pressedbuttonN`                | Which button was pressed, N is going to be incremented when a new button is pressed.  |
| `timebuttonN`                   | The different times in seconds at which the button was pressed since the start of the trial |
| `stimulusDuration`              | The different durations of each stimulus|

