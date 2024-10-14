---
layout: about
title: about
permalink: /

profile:
  align: left
  image: profile1.jpeg
  image_circular: false # crops the image to make it circular
  more_info: >
    Sungjun Sun Lee
    zinpolygon35@gmail.com

news: false # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page
---

I am interested in <b>HCI, with a focus on AR/VR and AI programming.</b> I enjoy creating software that combines these technologies, such as <b>educational programs or control systems that support collaboration.</b>

I am also interested in using <b>AI models like GPT and reinforcement learning to build human-AI interactions in virtual environments or user interfaces.</b> Rather than focusing on technical engineering or optimization, I aim to <b>explore new ideas for using AI and computer interaction to enhance education, productivity, and gaming in a human-centered way.</b>

My background includes research and development in AR/VR using Unity during both my undergraduate and graduate studies. During my undergraduate years, I made on <b>creating emotional interactions with AI-driven NPCs in an AR environment.</b> In my master's, I researched <b>reducing motion sickness in VR using sound, specifically studying whether reverse sound stimuli can help reduce motion sickness.</b>

I also have experience building various applications using <b>Python</b>, such as web applications with Flask and FastAPI, desktop software, automation scripts, chatbots, and trading systems. And I have an <b>experience of publishing mobile games ( 5 more ) and VR Game.</b> I am using Unity Engine for making games. Additionally, I have used <b>JavaScript</b> to develop APIs and automation servers, studied <b>smart contracts with Solidity for blockchain applications</b>, and <b>created over 50 trading indicators using Pinescript</b>.

<div class="clearfix"></div>

---

### Languages & Skills

<b><h5>Korean Fluency: Native speaker<h5></b>

<b><h5>English Fluency: Conversational +</h5></b>

<table border="1" cellpadding="10" cellspacing="0">
  <thead>
    <tr>
      <th>Technology</th>
      <th>Experience</th>
      <th>Keywords</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Python</strong></td>
      <td>7 years</td>
      <td>
        <ul>
          <li>Flask, FastAPI API System</li>
          <li>Chatbot</li>
          <li>Auto Trading System - MT5, Stocks, Crypto</li>
          <li>Scraping, Crawling</li>
          <li>Desktop App</li>
          <li>etc</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><strong>Unity</strong></td>
      <td>5 years</td>
      <td>
        <ul>
          <li>Mobile Game</li>
          <li>AR - ARCore, ARKit, Vuforia</li>
          <li>VR</li>
          <li>Applications</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><strong>Javascript</strong></td>
      <td>2-3 years</td>
      <td>
        <ul>
          <li>API System</li>
          <li>Web3 Application</li>
          <li>Automation System</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><strong>PineScript</strong></td>
      <td>3 years</td>
      <td>
        <ul>
          <li>Strategies</li>
          <li>Backtesting</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><strong>Solidity</strong></td>
      <td>1 year</td>
      <td>
        <ul>
          <li>Web3 Smart Contract</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

---

## Publications

<div class="publications">

{% bibliography %}

</div>

<div class="clearfix"></div>

---

## Education & Experience

<div class="education"></div>

<div class="education-section">
  {% assign education = site.data.resume.education %}
  <ul class="card-text font-weight-light list-group list-group-flush">
    {% for content in education %}
      <li class="list-group-item">
        <div class="row">
          <div class="col-xs-2 col-sm-2 col-md-2 text-center date-column">
            <table class="table-cv">
              <tbody>
                <tr>
                  <td>
                    {% if content.startDate and content.endDate %}
                      <span class="badge font-weight-bold danger-color-dark text-uppercase align-middle" style="min-width: 75px">
                        {{ content.startDate }} - {{ content.endDate }}
                      </span>
                    {% endif %}
                  </td>
                </tr>
              </tbody>
            </table>
          </div>
          <div class="col-xs-10 col-sm-10 col-md-10 mt-2 mt-md-0">
            <h6 class="title font-weight-bold ml-1 ml-md-4">{{ content.studyType }} in {{ content.area }}</h6>
            <h6 class="ml-1 ml-md-4" style="font-size: 0.95rem">
              <a href="{{ content.url }}" target="_blank">{{ content.institution }}</a>
            </h6>
            <p class="ml-1 ml-md-4" style="font-size: 0.85rem">{{ content.location }}</p>
            {% if content.score %}
              <p class="ml-1 ml-md-4" style="font-size: 0.85rem">Score: {{ content.score }}</p>
            {% endif %}
          </div>
        </div>
      </li>
    {% endfor %}
  </ul>
</div>

<div class="clearfix"></div>

---
