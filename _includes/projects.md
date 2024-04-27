<h2 id="publications" style="margin: 2px 0px -15px;">Undergraduate Projects</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.projects.main %}

<li>
<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    {% if link.image %} 
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=120%;height=50%">
    {% endif %}
    {% if link.conference_short %} 
    <abbr class="badge">{{ link.conference_short }}</abbr>
    {% endif %}
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
     
      <div class="author">{{ link.authors }}</div>
      <div class="periodical"><em>{{ link.conference }}</em>
      </div>
    <div class="links">
      {% if link.pdf %}
      {% if link.github %} 
       <p><i class="fab fa-fw fa-github" aria-hidden="true"></i> <a href="{{link.github}}"> GitHub</a>｜<svg t="1697827825990" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="7835" width="16" height="16"><path d="M645.071238 97.52381L828.952381 281.258667V414.47619h48.761905v390.095239h-48.761905v48.761904a73.142857 73.142857 0 0 1-73.142857 73.142857H268.190476a73.142857 73.142857 0 0 1-73.142857-73.142857v-48.761904H146.285714V414.47619h48.761905V170.666667a73.142857 73.142857 0 0 1 73.142857-73.142857h376.880762zM755.809524 804.571429H268.190476v48.761904h487.619048v-48.761904zM368.274286 520.94781H299.154286v174.445714h43.885714v-53.101714h10.971429a177.493333 177.493333 0 0 0 31.597714-2.852572 103.619048 103.619048 0 0 0 16.237714-4.827428c4.534857-2.048 8.777143-4.461714 12.726857-7.241143 7.168-5.412571 12.507429-12.141714 16.018286-20.187429 3.364571-8.484571 5.046857-17.334857 5.046857-26.550857a72.338286 72.338286 0 0 0-4.388571-23.698286 56.441905 56.441905 0 0 0-13.604572-19.968 62.025143 62.025143 0 0 0-23.917714-12.726857 116.784762 116.784762 0 0 0-25.453714-3.291428z m140.434285 0h-61.44v174.445714h61.44c6.875429-0.146286 13.750857-0.731429 20.626286-1.755429 6.144-1.024 12.141714-2.56 17.993143-4.608 5.266286-2.194286 10.313143-4.754286 15.140571-7.68 4.388571-3.218286 8.411429-6.875429 12.068572-10.971428 3.510857-4.388571 6.582857-9.069714 9.216-14.043429a110.689524 110.689524 0 0 0 6.144-16.896c2.194286-10.24 3.364571-20.626286 3.510857-31.158857a176.37181 176.37181 0 0 0-1.755429-21.284571 113.249524 113.249524 0 0 0-4.608-18.432 90.599619 90.599619 0 0 0-7.68-15.579429 78.214095 78.214095 0 0 0-10.532571-12.507429 77.994667 77.994667 0 0 0-13.604571-9.435428 93.42781 93.42781 0 0 0-16.457143-6.363429 139.702857 139.702857 0 0 0-30.061715-3.730285z m213.504 0h-116.736v174.445714h43.885715v-65.828572h63.414857v-34.011428h-63.414857v-39.497143h72.850285v-35.108571z m-206.482285 35.108571c4.973714 0.146286 9.654857 1.536 14.043428 4.169143 4.534857 3.072 8.265143 7.021714 11.190857 11.849143 3.218286 5.851429 5.485714 11.995429 6.802286 18.432 1.024 5.997714 1.609143 11.995429 1.755429 17.993143-0.146286 6.144-0.731429 12.214857-1.755429 18.212571a62.22019 62.22019 0 0 1-6.802286 18.212571c-2.925714 4.681143-6.656 8.557714-11.190857 11.629715a28.038095 28.038095 0 0 1-14.043428 3.730285h-24.576v-104.228571h24.576z m-151.625143 0c3.949714 0.146286 7.826286 0.877714 11.629714 2.194286 3.364571 1.316571 6.363429 3.218286 8.996572 5.705143 4.681143 5.12 7.021714 11.117714 7.021714 17.993142 0 7.314286-2.706286 13.385143-8.118857 18.212572a28.525714 28.525714 0 0 1-9.874286 5.485714 47.88419 47.88419 0 0 1-12.068571 1.536h-18.651429v-51.126857h21.065143z m217.307428-385.414095L268.190476 170.666667v243.809523h487.619048v-49.956571h-174.372572L581.412571 170.666667z m73.142858 39.740952v80.993524h81.042285l-81.042285-80.993524z" p-id="7836"></path></svg> <a href="{{link.pdf}}">PDF</a> 
</p>
      {% endif %}
      {% endif %}
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% endif %}
      {% if link.page %} 
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
      {% endif %}
      {% if link.bibtex %} 
      <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
      {% endif %}
      {% if link.notes %} 
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</div>
</li>

<br>

{% endfor %}


{% for link in site.data.projects.other %}

<li>
<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    {% if link.image %} 
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
    {% endif %}
    {% if link.conference_short %} 
    <abbr class="badge">{{ link.conference_short }}</abbr>
    {% endif %}
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
      <div class="author">{{ link.authors }}</div>
      <div class="periodical"><em>{{ link.conference }}</em>
      </div>
    <div class="links">
      {% if link.pdf %} 
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
      {% endif %}
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% endif %}
      {% if link.page %} 
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
      {% endif %}
      {% if link.bibtex %} 
      <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
      {% endif %}
      {% if link.notes %} 
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</div>
</li>

<br>

{% endfor %}

</ol>
</div>
