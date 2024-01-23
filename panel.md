---
layout: page
title: Panels
---

<html>
<script>

function getPanelSpeakersForPanelName(panelName) {
  // Filter all speakers to select only those that are in the given panel
  const speakers = {{ site.data.speakers | jsonify }};
  const panelSpeakers = speakers.filter(speaker => speaker.Panel !== undefined);
  return panelSpeakers.filter(speaker => (speaker.Panel && speaker.Panel.toLowerCase().includes(panelName.toLowerCase())));
}

function getUrlForSpeaker(speaker) {
  // Take website if available, then twitter, then github
  if (speaker.Website) {
    return speaker.Website;
  }
  if (speaker.Twitter) {
    return speaker.Twitter;
  }
  if (speaker.Github) {
    return speaker.Github;
  }

  return "";
}

function emptyStringForNull(element) {
  // Return empty string if the element is null to prevent the display of "null" on the page
  const out = element ? element : "";
  return out;
}

function getImageAssetPathForSpeaker(speaker) {
  // Retrieve image path of the speaker photo
  return `../img/speakers/${speaker.Name.toLowerCase().replaceAll(' ', '_')}.jpg`;
}

function formatSpeakerDiv(speaker) {
  // Generate a card for speaker with photo | name | panel job | affiliation | twitter | github
  // Only the speaker name is mandatory but you should check that there is a SURNAME_NAME.jpg
  // photo in the img/speakers folder
  // For the other fields, it only appears if the value is defined in the _data/speakers.csv
  if (!speaker.Name || speaker.Name === "") {
    return "";
  }

  const speakerUrl = getUrlForSpeaker(speaker);

  return `
    <div>
      <a style="color:#05323F" href="${speakerUrl}">
        <img src=${getImageAssetPathForSpeaker(speaker)} />

        <h3>${speaker.Name}</h3>
        ${speaker.Job ? `<h4>${speaker.Job}</h4>` : ""}
        ${speaker.Affiliation ? `<h6>${speaker.Affiliation}</h6>` : ""}
      </a>
      ${speaker.Twitter ? `<a target="_blank" href="${speaker.Twitter}"><i class="fa fa-twitter fa-2x"></i></a>` : ""}
      ${speaker.GitHub ? `<a target="_blank" href="${speaker.GitHub}"><i class="fa fa-github fa-2x"></i></a>` : ""}
    </div>
  `;
}

function displayPanel(panelName) {
  // Generate divs that contain all the speakers that are in the given panel
  const speakers = getPanelSpeakersForPanelName(panelName);
  return `${speakers.map(formatSpeakerDiv).join("")}`;
}

</script>
</html>


The OSR has always been a place to learn and share experiences.
This year we are centering these experiences around themes which are undergoing rapid change in our discipline.

## Topic 1: Telehealth as a tool for open data research and sharing
#### <a href="https://www.crowdcast.io/e/panel-1-telehealth" target="_blank">Join on Crowdcast</a> 
When: 8:00 GMT-4 | July 23, 2023 (Sunday) <br/>
<br/>
Neurological care is a challenge in any given situation, more so for those living in rural and suburban areas due to limited access. The usage of telemedicine and information and communication technology (ICT) can avail therapeutic measures to be instituted prior to transfer of patients to more urban hospices. Computerized image transfer and big data analysis to provide fast diagnostics in regions with limited resources are among the potential roles of neuroscience in impacting mainstream neurological management. This panel will focus on discussing the lessons learned that impact of telehealth in neurosciences, particularly in assisting fast diagnostics, improved post-surgical outcomes, and promotion of educational teleconferencing to enhance neurological services to the underprivileged and underserved rural community. It will also address on ways to leverage these tools to transmit data securely and explore how neuroscience has impacted telehealth practices worldwide. 
<br><br>
At the end of the panel discussion, the audience members will be able to:
1. Identify key roles of neuroscience in aiding the development and advancement of telehealth practices worldwide 
2. Able to recognize potential challenges and gain insight on ways to overcome these pertaining to telehealth services in neurological conditions
<br/>

<html>
<div class="panel-speakers" id="panel1"></div>

<script>
document.getElementById("open-science-panel").innerHTML = displayPanel("Open Science");
</script>
</html>

## Topic 2: Evolution of open publishing (To do or not to do?/Lessons learnt)
#### <a href="https://www.crowdcast.io/e/panel-2-evolution-of" target="_blank">Join on Crowdcast</a> 
When: 14:15 GMT-4 | July 23, 2023 (Sunday) <br/>
<br/>
The world of scientific publishing changed exponentially in the past decade: More journals join forces to recommend authors to upload their manuscripts to preprint servers; Code and data are required to be made publicly available for replication. At the same time, journals are providing open access options, sometimes exclusively, which means that authors must pay a large amount of money (e.g., up to €9,500) for publishing one single paper. Journals also seek for new publishing models. For instance, the online journal eLife is running a new model of no rejection after peer review. Our generation is facing the rapid evolution of research publishing. We have noticed that researchers have different thoughts on these changes. Topics will include but not limit to: cultural changes regarding assessment of funding and paper quality; what model is more accessible – higher publication fees & open access vs. reader fees; auxiliary materials that accompany papers. 
<br><br>
Questions adressed during this panel discussion will include:
- How do journals balance cost and benefit? 
- Have you benefited from the open materials (e.g., code and data) with published papers? And how do you deal with such materials of your own studies?
- Does a journal’s publishing model (e.g., APC) influence your decision to peer review?
- What are your thoughts about the future of peer review?
- As authors and reviewers, what do you think about eLife’s new model? What do you think is the best publishing model from the view of researchers?
<br>
<html>
<div class="panel-speakers" id="panel2"></div>

<script>
document.getElementById("open-publishing-panel").innerHTML = displayPanel("Open Publishing");
</script>
</html>


## Topic 3: Standardization of code
#### <a href="https://www.crowdcast.io/e/panel-3-standardization" target="_blank">Join on Crowdcast</a> 
When: 8:00 GMT-4 | July 24, 2023 (Monday) <br/>
<br/>
An increasing number of journals require a data and code availability statement to be included in a published paper. From the perspective of transparency, efficient use of time and resources, and replication of results, open code is very important. However, analysis code is often a second-class citizen in neuroimaging research. This is something we can change. In this session we will discuss with four experts best-practices in software development for scientists - and how those practices can result in real-world gains in research quality and output. Sharing code by making it available in some repository is only one step towards practicing open code. By adhering to certain standards, like good coding practices and quality monitoring, open code can contribute to efficiency and quality of research. We will share tips on best-practices for coding, discuss advantages and disadvantages of standardization of open code, and address the question of whether we can expect individual researchers/small labs to share code of a comparable standard as specialized programmers. 
<br>
<html>
<div class="panel-speakers" id="panel3"></div>

<script>
document.getElementById("open-code-panel").innerHTML = displayPanel("Open Code");
</script>
</html>


## Topic 4: Open Data Governance and Infrastructure
#### <a href="https://www.crowdcast.io/e/panel-4-data-governance" target="_blank">Join on Crowdcast</a> 
When: 10:30 GMT-4 | July 25, 2023 (Tuesday) <br/>
<br/>
The sharable open source data serves are the foundation of open science, requiring effective strategies for management and organization. As more and more data are accumulated, sustainable data usage requires interactions between front- and back-end engineers, scientists, data providers, and data users. A large amount of brain image data has been collected, anticipating solving the problems of varied data quality, limited funding resources, or having too little data for studying specific populations or rare diseases in neuroscience research. Taking the advantage of methodologies like AI, big data and multi-omics approaches, on the other hand, enables scientists and doctors to understand the brain from new perspectives. By establishing discussions in this panel session, we take large-scale opensource brain image datasets as examples and aim to reduce inequalities by promoting value-added data usage with experts from different domains. Moreover, the panel will also include discussions on legal and ethical issues.
<br><br>
At the end of the panel discussion, the audience members will be able to:
1. Acquire the information on the current available opensource brain image database.
2. Understand how to properly use or collect open brain image data ethically and legally.  
3. Adopt value-added strategies and infrastructure to achieve data sustainability.  
<br>
<html>
<div class="panel-speakers" id="panel4"></div>

<script>
document.getElementById("statistical-perspectives-panel").innerHTML = displayPanel("Statistical Perspectives");
</script>
</html>

## Topic 5: Large open data repositories: sustainability and global implications of reuse
#### <a href="https://www.crowdcast.io/e/panel-5-data-reuse" target="_blank">Join on Crowdcast</a> 
When: 10:30 GMT-4 | July 26, 2023 (Wednesday) <br/>
<br/>
In this session we will discuss pros and cons of reusing large open data sets. There are many advantages of large neuroimaging-based databases, however, most involve data from the Western, educated, industrial population. We will discuss the implications of this. Another aspect we want to discuss is the support for data storage, sharing, and future reuse. There is a growing need for assistance through data managers or data librarians, free but monitored access to open data repositories for both long-term and short-term storage, as well as educational programs to increase awareness and to help create a culture of good data practices in neuroscience. 
<br>

<html>
<div class="panel-speakers" id="panel5"></div>

<script>
document.getElementById("social-bias-panel").innerHTML = displayPanel("Social Bias");
</script>
</html>
