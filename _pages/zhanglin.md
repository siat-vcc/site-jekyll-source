---
title: "Zhanglin Cheng"
layout: person
excerpt: "Zhanglin Cheng's page"
sitemap: false
permalink: /person/zhanglin.html
---
<script type="text/javascript">
function showInfo()
{
document.getElementById('infoDiv').style.display='block';
document.getElementById('pubDiv').style.display='none';
document.getElementById('projectDiv').style.display='none';
document.getElementById('honorDiv').style.display='none';

document.getElementById('infoTitle').style.fontWeight = 'bold';
document.getElementById('pubTitle').style.fontWeight = 'normal';
document.getElementById('projectTitle').style.fontWeight = 'normal';
document.getElementById('honorTitle').style.fontWeight = 'normal';
}
function showPub()
{
document.getElementById('infoDiv').style.display='none';
document.getElementById('pubDiv').style.display='block';
document.getElementById('projectDiv').style.display='none';
document.getElementById('honorDiv').style.display='none';

document.getElementById('infoTitle').style.fontWeight = 'normal';
document.getElementById('pubTitle').style.fontWeight = 'bold';
document.getElementById('projectTitle').style.fontWeight = 'normal';
document.getElementById('honorTitle').style.fontWeight = 'normal';
}
function showProject()
{
document.getElementById('infoDiv').style.display='none';
document.getElementById('pubDiv').style.display='none';
document.getElementById('projectDiv').style.display='block';
document.getElementById('honorDiv').style.display='none';

document.getElementById('infoTitle').style.fontWeight = 'normal';
document.getElementById('pubTitle').style.fontWeight = 'normal';
document.getElementById('projectTitle').style.fontWeight = 'bold';
document.getElementById('honorTitle').style.fontWeight = 'normal';
}
function showHonor()
{
document.getElementById('infoDiv').style.display='none';
document.getElementById('pubDiv').style.display='none';
document.getElementById('projectDiv').style.display='none';
document.getElementById('honorDiv').style.display='block';

document.getElementById('infoTitle').style.fontWeight = 'normal';
document.getElementById('pubTitle').style.fontWeight = 'normal';
document.getElementById('projectTitle').style.fontWeight = 'normal';
document.getElementById('honorTitle').style.fontWeight = 'bold';
}
</script> 
<link rel="stylesheet" type="text/css" href="{{ site.url }}{{ site.baseurl }}/css/person.css" media="all" />

<div markdown="0" id="left" style="display:inline-block;width: 20%;margin: 0;vertical-align:top;" class="contentFont">
        <div>
            <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/chengzhanglin.jpg" width="70%" style="margin:0 auto"/>
        </div>
        <p>
            <b style="font-weight:bold; font-size:20px">Zhanglin Cheng</b><br/>
            <b style="font-weight:bold; font-size:17px">程章林</b>
        </p>
        <p>
        <b>Associate Professor</b><br>
        <a href="http://www.siat.cas.cn/jgsz2016/jgdh2016/kybm2016/ygs2016/yjdy20161/yxtxyszssyjs2016/zxjj_125385/" style="font-size:13px">Research Lab for Medical Imaging and Digital Surgery</a><br/>
        <a href="http://www.siat.ac.cn/" style="font-size:13px">Shenzhen Institutes of Advanced Technology</a><br/>
        <a href="http://www.cas.cn/" style="font-size:13px">Chinese Academy of Sciences</a>
        </p>
        <p style="font-size:14px">mail: <i>zl.cheng at siat.ac.cn</i><br/></p>
        <p>
            <a href="https://scholar.google.com/citations?user=VXKK9ncAAAAJ&hl">
                <img src="{{ site.url }}{{ site.baseurl }}/images/logopic/gscholar.png" width="25px" style="float:left;margin-left:30px;margin-right:12px;" align="left" />
            </a>
            <a href="http://people.ucas.edu.cn/~chengzhanglin">
                <img src="{{ site.url }}{{ site.baseurl }}/images/logopic/caslogo.jpg" width="25px" style="float:right;margin-right:90px;" align="right" />
            </a>
        </p>
</div>
<div markdown="0" id="right" style="display:inline-block;width: 70%;margin: 10px;vertical-align:top;" class="contentFont">
        <nav id="nav">
            <a id="infoTitle" onclick="showInfo()">ABOUT</a> &nbsp;&nbsp;&nbsp;&nbsp;
            <a id="pubTitle" onclick="showPub()">PUBLICATIONS</a> &nbsp;&nbsp;&nbsp;&nbsp;
            <a id="projectTitle" onclick="showProject()">PROJECTS</a> &nbsp;&nbsp;&nbsp;&nbsp;
            <a id="honorTitle"  onclick="showHonor()">HONOR</a> &nbsp;&nbsp;&nbsp;&nbsp;
        </nav>
        <br/>
        <div markdown="0" id="infoDiv" style="margin: 10px;vertical-align:top;" class="shadowDiv">
            Zhanglin Cheng is a associate professor at Shenzhen Institues of Advanced Technology, Chinese Academy of Sciences. 
        </div>
        <div markdown="0" id="pubDiv" style="margin: 10px;vertical-align:top;" class="shadowDiv">
            {% assign year = 2049 %}
            {% for publi in site.data.czlJournal %}
            {% if year > publi.year %}
            {% assign year = publi.year %}
            <h4>{{ publi.year }}</h4>
            {% endif %}
            <b>{{ publi.title }}</b> <br />
            <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
            <br/><br/>
            {% endfor %}
        </div>
        <div markdown="0" id="projectDiv" style="margin: 10px;vertical-align:top;" class="shadowDiv">
            {% for project in site.data.czlProjects %}
            <b>{{ project.title }}</b> <br />
            <em>{{ project.type }} </em><br />
            {{ project.info }}<br/>
            <!-- {{ project.role }}<br/> -->
            <br/>
            {% endfor %}
        </div>
        <div markdown="0" id="honorDiv" style="margin: 10px;vertical-align:top;" class="shadowDiv">
            this is his honor
        </div>
</div>
<script>
showInfo();
</script>
<br>
<br>