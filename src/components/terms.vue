<template>
  <div class="cat-terms container-fluid">
    <div class="row">
      <div class="col-sm">
        <div class="cat-header">
          <div class="row">
            <div class="cat-title col-sm-12">
              <p>Terms of Conduct</p>
            </div>
            <div class="cat-subtitle col-sm-4 offset-sm-4">
              <p>
                <strong>IMPORTANT:</strong> By registering your participation you agree to the terms and conditions presented
                below. The CSE Hackathon follows the academic moral, ethics
                and decency standards. Responsible behaviour is expected.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="cat-body col-sm-8 offset-sm-2">
        <ol>
          <li>
            <span class="cat-section">Code of conduct</span>:
          </li>
          <ul>
            <li>
              Participants shall refrain from creating any content that could be considered illegal and/or
              obscene, offensive, defamatory, indecent, pornographic, unsuitable, racist, xenophobic or
              in any other way objectionable in line with general moral standards and/or according to the
              decision of the CSE Hackathon Organization Committee or that would/could damage the reputation
              of Chalmers and the University of Gothenburg.
            </li>
            <li>
              Participants shall refrain from accessing, storing (saving) and sending content or data with
              illegal, copyright-infringing, sexist, racist, offensive or otherwise objectionable ideologies.
            </li>
            <li>
              Participants shall comply with the house rules in force at the event location as well as any
              instructions given by the organizers on location, and shall neither enter nor use any rooms,
              installations or systems at the event location that are not intended to be used as part of
              the event.
            </li>
            <li>
              Participants assume responsibility for any damage they cause to the premises, installations and
              systems at the event location. In this respect and to the extent permitted by law, the CSE
              Hackathon organization committee declines all liability.
            </li>
          </ul>
          <hr>
          <li>
            <span class="cat-section">Participation</span>:
          </li>
          <ul>
            <li>
              Participants need to register before deadline of
              <strong>April 30, 2018</strong>. However, the registration follows a first come, first served principle.
              When the maximum number of participants is reached, the registration page will reflect that
              new registrations are marked as reserves.
            </li>
            <li>
              Only students enrolled in the Bachelor Programmes from the University of Gothenburg are allowed
              to register and compete in the event.
            </li>
            <li>
              Teams will have at most 4 participants. Individuals can only participate in one team. The entire
              team shall be present at the hackathon, with the exception of force majeure.
            </li>
            <li>
              Participants will need to bring their own computers, mobile phones and any other devices with
              the necessary software.
            </li>
          </ul>
          <hr>
          <li>
            <span class="cat-section">Your creation(s)</span>;
          </li>
          <ul>
            <li>
              Participants are allowed to reuse their own code and libraries, but the competing project has
              to be new and created during the CSE Hackathon.
            </li>
            <li>Participants are prepared to present the results of their work at the end of the CSE Hackathon.</li>
            <li>Participants must clearly reference all sources/source materials when presenting the results.</li>
            <li>At the end of the hackathon, participants must describe what was developed during the hackathon.</li>
            <li>
              Participants are the owner of their creations. By participating at the hackathon the research
              projects at the Computer Science and Engineering Department at Chalmers and the University
              of Gothenburg are granted the right of using your application for research, but not commercial,
              purposes. Research use could include testing the application with a large user group, or
              investigating its effect on learning and explore further improvements of its core concept.
            </li>
            <li>
              Participants understand and acknowledge that the CSE Hackathon Organization Committee may have
              developed or commissioned, or may develop in the future, materials similar to the participants’
              work. Participants waive any and all claims they may have resulting from any similarities
              between their creations and any such materials.
            </li>
          </ul>
        </ol>
      </div>
    </div>
  </div>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Anton|Inconsolata|Roboto+Slab");

.cat-terms {
  color: white;
  padding-top: 5%;
  padding-bottom: 5%;
}

.cat-header {
  margin: 0vh 0vw 5vh 0vw;
}
.cat-title {
  font-family: "Roboto Slab", serif;
  font-weight: bold;
  font-size: 5em;
  text-align: center;
}

.cat-subtitle {
  font-family: "Inconsolata", monospace;
  font-weight: bold;
  font-size: 1.5em;
  text-align: center;
}

.cat-subtitle strong {
  color: red;
}

.cat-section {
  color: red;
  font-family: "Inconsolata", monospace;
  font-weight: bold;
  font-size: 1.5em;
}

.cat-body {
  /* border: 1px double red; */
  font-family: "Inconsolata", monospace;
  font-size: 1.2em;
}

.cat-body > ul > li {
  padding: 2% 0%;
}
</style>
