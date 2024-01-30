---
layout: page
title: Schedule
---


<script>
const ALL_DAYS = ["07-23", "07-24", "07-25", "07-26"];

function setupActiveDayTab(activeDay) {
    /* First, remove the "active" classname for all tabs */
    ALL_DAYS.forEach(day => {
        let divDay = document.getElementById(`day-${day}`);
        divDay.className = divDay.className.replace("active", "");
    });
    
    /* Then add it to the appropriate day */
    let divDay = document.getElementById(`day-${activeDay}`);
    divDay.className = `${divDay.className} active`;
}

function setupActiveDaySchedule(activeDay) {
    /* First, hide all the schedule blocks */
    ALL_DAYS.forEach(day => {
        let divDay = document.getElementById(`schedule-${day}`);
        divDay.className = divDay.className.replace("active", "");
    });
    
    /* Then display:block to show the appropriate one */
    let divDay = document.getElementById(`schedule-${activeDay}`);
    divDay.className = `${divDay.className} active`;
}

function showScheduleForDay(day) {
    setupActiveDayTab(day);
    setupActiveDaySchedule(day);
}
</script>

<div class="schedule-days">
  <div id="day-06-24" class="schedule-day active" onclick="showScheduleForDay('06-24')">June 24</div>
  <div id="day-06-25" class="schedule-day" onclick="showScheduleForDay('06-25')">June 25</div>
  <div id="day-06-26" class="schedule-day" onclick="showScheduleForDay('06-26')">June 26</div>
  <div id="day-06-27" class="schedule-day" onclick="showScheduleForDay('06-27')">June 27</div>
</div>

<h5 style="text-align: center;">
GMT+9
</h5>

## Coming soon!
Meanwhile, please find the information in the following sections:
* [Panel Discussions](/panel.md)
* [Table Talk](/tabletalk.md)
* [Emergent Sessions](/emergent.md)
* Symposium to-be-confirmed

<div id="schedule-06-24" class="schedule-block">
    <h4>June 24, Monday</h4>
    <div class="schedule-content">
        <table class="osr-schedule">
            <!-- <tr>
                <td>GMT+9</td>
                <td>OPEN SCIENCE ROOM</td>
            </tr>
            <tr>
                <td>8:00-9:00</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/panel/" target="_blank">Panel:</a> Telehealth as a tool for open data research and sharing</div>
                    <div><a href="https://www.crowdcast.io/e/panel-1-telehealth" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>
            <tr>
                <td>10:30-11:30</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/emergent/" target="_blank">Emergent Session:</a> BIDS Townhall</div>
                    <div><a href="https://www.crowdcast.io/e/osr-2023-emergent-1" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>
            <tr>
                <td>11:30-12:15</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/tabletalk/" target="_blank">Table Topic Discussion:</a> Telehealth as a tool for open data research and sharing in neurosciences</div>
                    <div><a href="https://www.crowdcast.io/e/osr-table-telehealth" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>
            <tr>
                <td>14:15-15:30</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/panel/" target="_blank">Panel:</a> Evolution of Open Publishing (To do or not to do? Lessons learnt!)</div>
                    <div><a href="https://www.crowdcast.io/e/panel-2-evolution-of" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>
            <tr>
                <td>16:45-17:30</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/tabletalk/" target="_blank">Table Topic Discussion:</a> Evolution of Open Publishing</div>
                    <div><a href="https://www.crowdcast.io/e/osr-table-evolution-of" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr> -->
        </table>
    </div>
</div>

<div id="schedule-06-25" class="schedule-block">
    <h4>June 25, Tuesday</h4>
    <div class="schedule-content">
        <table class="osr-schedule">
            <!-- <tr>
                <td>GMT+9</td>
                <td>OPEN SCIENCE ROOM</td>
            </tr>
            <tr>
                <td>8:00-9:00</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/panel/" target="_blank">Panel:</a> Standardization of Code (tips)</div>
                    <div><a href="https://www.crowdcast.io/e/panel-3-standardization" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>
            <tr>
                <td>10:30-11:30</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/emergent/" target="_blank">Emergent Session:</a> Developing a community-driven standard file format for brain tractography</div>
                    <div><a href="https://www.crowdcast.io/e/osr-2023-emergent-2" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>
            <tr>
                <td>12:15-13:00</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/tabletalk/" target="_blank">Table Topic Discussion:</a> Standardization of Code</div>
                    <div><a href="https://www.crowdcast.io/e/osr-table-standardization" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>
            <tr>
                <td>14:45-15:45</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/emergent/" target="_blank">Emergent Session:</a> Discuss ideas for longitudinal simulated datasets for interplay of brain, behavior, and cognition</div>
                    <div><a href="https://www.crowdcast.io/e/osr-2023-emergent-3" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr> -->
        </table>
    </div>
</div>

<div id="schedule-07-26" class="schedule-block">
    <h4>June 26, Wednesday</h4>
    <div class="schedule-content">
        <table class="osr-schedule">
            <!-- <tr>
                <td>GMT+9</td>
                <td>OPEN SCIENCE ROOM</td>
            </tr>
            <tr>
                <td>8:00-9:00</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/emergent/" target="_blank">Emergent Session:</a> Enabling federated analysis on large datasets with COINSTAC Vaults</div>
                    <div><a href="https://www.crowdcast.io/e/osr-2023-emergent-4" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>
            <tr>
                <td>8:00-9:15</td>
                <td>
                    <div>Morning Symposia: Open Science - sustainability through success stories</div>
                </td>
            </tr>
            <tr>
                <td>10:30-11:30</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/panel/" target="_blank">Panel:</a> Open Data Governance and Infrastructure</div>
                    <div><a href="https://www.crowdcast.io/e/panel-4-data-governance" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>
            <tr>
                <td>11:45-12:45</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/tabletalk/" target="_blank">Table Topic Discussion:</a> Open Data Governance and Infrastructure - Sharable Resources in Neuroimaging</div>
                    <div><a href="https://www.crowdcast.io/e/osr-table-data-governance" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>
            <tr>
                <td>14:00-14:30</td>
                <td>
                    <div>Off Schedule Session: Mathworks</div>
                    <div><a href="https://www.crowdcast.io/c/osr-mathworks" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>           
            <tr>
                <td>14:45-16:15</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/emergent/" target="_blank">Emergent Session:</a> Physiopy open meeting: physiology community practices + Challenges for small collaborative software projects</div>
                    <div><a href="https://www.crowdcast.io/e/osr-2023-emergent-5" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr> -->
        </table>
    </div>
</div>
<div id="schedule-06-27" class="schedule-block">
    <h4>June 27, Thursday</h4>
    <div class="schedule-content">   
        <table class="osr-schedule">
            <!-- <tr>
                <td>GMT+9</td>
                <td>OPEN SCIENCE ROOM</td>
            </tr>
            <tr>
                <td>10:30-11:30</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/panel/" target="_blank">Panel:</a> Large open data repositories: sustainability and global implications of reuse</div>
                    <div><a href="https://www.crowdcast.io/e/panel-5-data-reuse" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr>
            <tr>
                <td>11:45-12:45</td>
                <td>
                    <div><a href="https://ohbm.github.io/osr2023/tabletalk/" target="_blank">Table Topic Discussion:</a> Large open data repositories: sustainability and global implications of reuse</div>
                    <div><a href="https://www.crowdcast.io/e/osr-table-data-reuse" target="_blank">Join on Crowdcast</a></div>
                </td>
            </tr> -->
        </table>
    </div>
</div>

<div class="schedule-leave-space-before-footer">
</div>

<script>!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0];if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src='https://plugins.eventable.com/eventable.js';fjs.parentNode.insertBefore(js,fjs);}}(document,'script', 'eventable-script');</script>

