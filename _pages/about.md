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

#### Languages & Skills

<b>Korean Fluency: Native speaker | English Fluency: Conversational +</b>

---

<b>Python | Unity | Javascript | Solidity | Pinescript </b>

---

### Publications

<div class="publications">

{% bibliography %}

</div>

<div class="clearfix"></div>

---

### Education & Experience

---

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

### Projects

<div class="post">

  <ul class="post-list">
    {% if page.pagination.enabled %}
      {% assign postlist = paginator.posts %}
    {% else %}
      {% assign postlist = site.posts %}
    {% endif %}
    
    {% for post in postlist %}


    <li>

      {% if post.thumbnail %}
      <div class="row">
        <div class="col-sm-9">
      {% endif %}
          <h3>
            {% if post.redirect == blank %}
              <a class="post-title" href="{{ post.url | relative_url }}">{{ post.title }}</a>
            {% elsif post.redirect contains '://' %}
              <a class="post-title" href="{{ post.redirect }}" target="_blank">{{ post.title }}</a>
            {% else %}
              <a class="post-title" href="{{ post.redirect | relative_url }}">{{ post.title }}</a>
            {% endif %}
          </h3>
          <p>{{ post.description }}</p>
          <p class="post-tags">
          </p>
        </div>
        {% if post.thumbnail %}
          <div class="col-sm-3">
            <img class="card-img" src="{{post.thumbnail | relative_url}}" style="object-fit: cover; height: 90%" alt="image">
          </div>
        </div>
      {% endif %}
    </li>

    {% endfor %}

  </ul>

</div>
<div class="clearfix"></div>
